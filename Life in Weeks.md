# Life in Weeks —— 用「周」为单位可视化人生

来源：https://github.com/busterbenson/notes/blob/master/_pages/life-in-weeks.md
（Buster Benson 的个人博客/笔记仓库）

## 这是什么

灵感来自 Tim Urban 在 Wait But Why 上的文章 *Your Life in Weeks*：把人的一生（假设活到 90 岁左右）画成一个网格，
**每一个小方格代表一周**。90 年 ≈ 4700 多周，整张图看起来密密麻麻，但一眼就能看出：

- 已经过去的周 vs. 还剩下的周（今天所在的位置一目了然）
- 人生被切分成一个个「十年」区块（20 多岁、30 多岁……），比抽象的「还有 60 年」更有冲击力
- 在特定的周上标注人生事件（出生、上学、搬家、结婚、亲人去世、换工作……），
  于是这张网格同时也变成了一份「个人编年史」

## Buster Benson 原版是怎么实现的

他在页面正文里直接写明了实现方式：

> a data file, a template, and a blog post mashed together on a Jekyll blog hosted on Netlify

拆开看是三个部分：

1. **数据文件** `_data/life-in-weeks.yml`
   一个以日期为 key 的 YAML 文件，每个日期下面挂一个或多个事件：
   ```yaml
   '1976-05-28':
     - name: "I enter the world"
       desc: "Born at Hoag Hospital in Newport Beach California..."
       category: "self"

   '1993-10-30':
     - name: "💔 My father passes away"
       desc: "From complications with treatment for lung cancer."
       category: "family"
       tags: ["dad"]
   ```
   `category` 决定方格的颜色分类，`desc`/`link`/`tags` 用于弹出的详情气泡（popover）。

2. **模板** `_layouts/life-in-weeks.html`
   一个 Jekyll/Liquid 模板：
   - 从 front matter 里读出 `start_date`（出生日期）和 `end_year`（画到哪一年，比如 2076）
   - 按「年」循环，每年再按「周」循环，逐周输出一个 `<div class="week">`
   - 每隔十年插入一个装饰性的分区标题（"My 20s"、"My 30s"…），并做了 sticky header
   - 用 JS 计算「今天」在第几周，之前的方格标记为已过去，之后的标记为 `future-date`
   - 如果某一周在数据文件里能查到事件，就把方格染色，并用 Bootstrap popover 展示 name/desc/link/图片

3. **页面本身** `_pages/life-in-weeks.md`
   只是一个很薄的 Markdown 页面，front matter 里指定 `layout: life-in-weeks` 和
   `data: life-in-weeks`，正文只有一段引言文字——真正的渲染逻辑全在上面两层。

整个仓库是标准 Jekyll 博客结构，托管在 Netlify 上，靠 Jekyll 的静态站点生成把「YAML 数据 + Liquid 模板」编译成最终的 HTML。

## 我怎么才能做一个自己的

原版依赖一整套 Jekyll 博客（`_config.yml`、`_data/`、`_layouts/`、Ruby/Bundler 环境），
如果只是想要「一张自己的人生周历」，没必要照搬整套建站流程。核心逻辑其实很简单：

```
for 每一周 from 出生日期 to 结束日期:
    画一个方格
    如果这一周 <= 今天: 标记为「已过去」
    如果这一周落在事件数据里: 染色 + 显示详情
    每 10 年画一次分组标题
```

这套逻辑用一个**单文件、零依赖的 HTML**就能实现，不需要 Jekyll/Ruby/构建工具，
双击就能在浏览器里打开，也可以直接扔进任何静态网站（包括 GitHub Pages）。

我已经在本仓库里放了一份这样的模板：**`life-in-weeks.html`**。

### 怎么用

1. 打开 `life-in-weeks.html`，找到顶部的 `CONFIG` 和 `EVENTS`（用注释标出了 `EDIT ME` 的区域）。
2. 把 `CONFIG.birthDate` 改成你自己的出生日期，`CONFIG.endYear` 改成你想画到哪一年
   （比如出生年份 + 90，代表按 90 岁的人生跨度来画）。
3. 在 `EVENTS` 里按 `'YYYY-MM-DD': [{ name, desc, category, link }]` 的格式加入你自己的人生事件
   （生日、开学、搬家、换工作……随意）。
4. 直接用浏览器打开这个 html 文件即可看到效果：
   - 每个小方格代表一周，按十年分组
   - 已经走过的周会有一层「已过去」的底色，「今天」所在的方格会高亮
   - 有事件的周会按 `category` 染色，鼠标悬停/点击可以看到事件详情
   - 顶部有图例（legend），说明每种颜色代表的分类

不需要装任何东西、不需要 Jekyll、不需要联网，改完 CONFIG/EVENTS 保存刷新即可。
