- [1. 使用 Raspberry Pi Pico 制作任意波发生器](#1-使用-raspberry-pi-pico-制作任意波发生器)

<div STYLE="page-break-after: always;"></div>

# 1. 使用 Raspberry Pi Pico 制作任意波发生器
一个很有意思的使用pico制作任意波形发生器的项目，主要需要材料如下：
- Raspberry pi pico microcontroller with male pin headers
- 1 5x7cm prototype board
- 2 20-pin female pin headers
- 23 resistors of identical value, near 2kOhm
相关示意图
![](/picture/F3WUUI0KKY0JSMW.webp)
![](/picture/F6Z9RB0KKY0JU0D.webp)
![](/picture/F8RIICRKKY0JU0B.webp)
![](/picture/FUH1QK9KKY0JU0A.webp)
![](/picture/FYYDWX2KKY0JSLL.webp)
代码包括
- DMA 的配置
- PIO 的配置和编程
- 用波形填充数组
- 启动 DMA。

此时波形已生成，pico 的 CPU 可自由执行其他任务。总线上会有数据通信，但 pico 具有高度并行的总线结构，我预计不会出现明显的速度减慢。

<https://www.instructables.com/Arbitrary-Wave-Generator-With-the-Raspberry-Pi-Pic/>
<div STYLE="page-break-after: always;"></div>
