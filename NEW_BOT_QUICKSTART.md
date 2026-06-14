# NEW_BOT_QUICKSTART.md

## 新建一个独立 bot 的标准流程

### 第一步：去 Telegram 创建 bot

找 **@BotFather**，发送：

```text
/newbot
```

按提示填写：

- bot 名字
- bot username

最后它会给你一个 **token**，先保存好。

---

## 第二步：在树莓派上跑创建脚本

### 示例：创建一个求职 bot

```bash
AGENT_ID="career" \
AGENT_NAME="Career" \
NEW_ACCOUNT_ID="Career_Lyu_bot" \
NEW_BOT_NAME="Career" \
bash /home/basteng/.openclaw/workspace/scripts/create_independent_bot_agent.sh
```

### 这几个变量的含义

#### `AGENT_ID`
- 机器用
- 全小写
- 尽量不带符号
- 例子：
  - `career`
  - `news`
  - `stockradar`

#### `AGENT_NAME`
- 给人看的 agent 名
- 例子：
  - `Career`
  - `News`
  - `Stock Radar`

#### `NEW_ACCOUNT_ID`
- 对应 Telegram bot username
- 最好和 Telegram 的 username 一致
- 例子：
  - `Career_Lyu_bot`
  - `News_Lyu_bot`

#### `NEW_BOT_NAME`
- 给人看的 bot 显示名
- 通常和 `AGENT_NAME` 一样
- 例子：
  - `Career`
  - `News`

---

## 第三步：输入 token

运行脚本后会提示：

```text
Enter bot token for Career_Lyu_bot:
```

把 **BotFather 给你的 token** 粘贴进去，回车。

---

## 第四步：给 bot 发一条消息

打开 Telegram，找到刚创建的 bot，发送任意一条消息，例如：

```text
hi
```

> 这一步必须做。  
> 不然 bot 没法主动给你发消息。

---

## 第五步：验证 bot 和 agent 绑定成功

在树莓派终端运行：

```bash
openclaw agents bindings
```

如果你能看到类似：

- `Career`
- `Career_Lyu_bot`

就说明它们已经接上了。

---

## 如果你以后要把某个 cron 推送切到这个 bot

### 第六步（可选）：切换 cron 到新 bot

使用第二个脚本：

```bash
bash /home/basteng/.openclaw/workspace/scripts/switch_cron_bot.sh \
  "你的cron任务名" \
  "Career_Lyu_bot"
```

### 示例
把午间新闻切到 `News_Lyu_bot`：

```bash
bash /home/basteng/.openclaw/workspace/scripts/switch_cron_bot.sh \
  "每日新闻中午推送" \
  "News_Lyu_bot"
```

### 这个脚本会自动做什么
- 改 live cron
- 改 desired cron
- 验证两边一致
- 自动 commit

---

## 以后你只要记住 2 个脚本

### 1. 新建 bot + agent
```bash
/home/basteng/.openclaw/workspace/scripts/create_independent_bot_agent.sh
```

### 2. 把某个 cron 切到某个 bot
```bash
/home/basteng/.openclaw/workspace/scripts/switch_cron_bot.sh
```

---

## 命名规则（最简单记法）

### 推荐规则

#### `AGENT_ID`
- 全小写
- 尽量别加短横杠
- 例子：
  - `career`
  - `news`
  - `stockradar`

#### `AGENT_NAME`
- 人类可读
- 例子：
  - `Career`
  - `News`
  - `Stock Radar`

#### `NEW_ACCOUNT_ID`
- 和 Telegram bot username 一样
- 例子：
  - `Career_Lyu_bot`
  - `News_Lyu_bot`
  - `Stock_Radar_Lyu_bot`

#### `NEW_BOT_NAME`
- 人类可读
- 通常和 `AGENT_NAME` 一样
- 例子：
  - `Career`
  - `News`
  - `Stock Radar`

---

## 一个完整例子

### 创建 Career bot

#### 1. 去 BotFather 创建
拿到：

- username：`Career_Lyu_bot`
- token：`xxxx`

#### 2. 在树莓派上运行

```bash
AGENT_ID="career" \
AGENT_NAME="Career" \
NEW_ACCOUNT_ID="Career_Lyu_bot" \
NEW_BOT_NAME="Career" \
bash /home/basteng/.openclaw/workspace/scripts/create_independent_bot_agent.sh
```

#### 3. 输入 token
脚本会提示：

```text
Enter bot token for Career_Lyu_bot:
```

#### 4. 去 Telegram 给 bot 发一句

```text
hi
```

#### 5. 验证绑定

```bash
openclaw agents bindings
```

#### 6. （如果要切任务）再运行

```bash
bash /home/basteng/.openclaw/workspace/scripts/switch_cron_bot.sh \
  "某条求职相关任务名" \
  "Career_Lyu_bot"
```

---

## 一句话总结

> **BotFather 创建 → 树莓派跑 create 脚本 → 给 bot 发一句 hi → 需要时再跑 switch 脚本切 cron。**
