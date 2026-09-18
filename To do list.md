# To Do List

记录想做的事情，完成后勾选。

## 待办

- [ ] **股票下单本地时间校准实验**：起因是[集思录讨论帖](https://www.jisilu.cn/question/524979?show_all_answer-TRUE__item_id-5534295__answer_id-5534295__single-TRUE#!answer_5534295)里关于下单时间校准的争论——NTP 校时约 ±10ms，瓶颈在网络抖动，更可靠的方案是用便宜的 USB GPS 模块（VK-162，约20元）配合 `gpsd` + `chrony` 校准本地时钟到毫秒级。手头有一块跑通 PTP 硬件时间戳的 FPGA 网卡（AS02MC04 / XCKU3P，taxi/Corundum 框架），可以顺手验证 GPS 授时精度，并延伸用网卡硬件时间戳量化本机网络处理延迟。分两阶段：阶段1（纯软件，GPS+chrony，验证本地时钟精度，一两天出结果）→ 根据结果决定是否投入阶段2（接入 FPGA GPIO 标定 PTP 时钟域偏差，对比硬件/软件时间戳量化处理延迟）。

## 已完成

- [ ]
