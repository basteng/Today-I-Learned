## FinFET CMOS 制造工艺流程表格

You are absolutely right! My apologies.  The markdown table formatting failed for steps 2-7 in my previous response.  I'm still under development and learning to handle complex formatting consistently.


I'll provide the complete table correctly formatted this time.  It's difficult to perfectly align everything due to the varying lengths of descriptions, but this should be much clearer:


| 步骤 | 子步骤 | 描述 | 图表 | 主要技术 | 备注 |
|---|---|---|---|---|---|
| **1. 晶圆准备** | 晶圆清洗 | 清洗硅晶圆 | Fig. 3.9(a) |  |  |
|  | 垫氧化物生长 | 在硅表面生长薄的SiO₂层 | Fig. 3.9(a) | 热氧化 |  |
|  | SiN 沉积 | 在垫氧化物上沉积SiN层，作为硬掩膜(HM) | Fig. 3.9(a), (b) | ALD/CVD | SiN 作为鳍片形成的硬掩膜和CMP终止层 |
|  | SADP 虚拟图案层沉积 | 在SiN上沉积SADP层 | Fig. 3.9(b) | ALD/CVD | 用于双倍图案密度 |
|  | 光刻胶涂覆 | 在SADP层上涂覆光刻胶 | Fig. 3.9(b) | 光刻 |  |
| **2. 鳍片图案化** | 虚拟图案刻蚀 | 刻蚀SADP虚拟图案至SiN表面 | Fig. 3.10(a) | 干法刻蚀 |  |
|  | 光刻胶去除 | 去除光刻胶 | Fig. 3.10(b) |  |  |
|  | 介质层沉积 | 沉积保形介质层 | Fig. 3.10(c) | ALD/CVD |  |
|  | 间隔物刻蚀 | 垂直刻蚀介质层，形成间隔物 | Fig. 3.10(d) | 干法刻蚀 |  |
|  | 虚拟图案去除 | 去除虚拟图案 (例如，使用KOH去除a-Si) | Fig. 3.10(e) | 化学刻蚀 |  |
| **3. 鳍片刻蚀** | 光刻胶涂覆和掩模对准 | 涂覆光刻胶并应用掩模 | Fig. 3.11(a) | 光刻 |  |
|  | 间隔物选择性刻蚀 | 选择性刻蚀间隔物 | Fig. 3.11(a) | 各向异性干法刻蚀 | 高选择性，最小化SiN HM损耗 |
|  | 光刻胶去除 | 去除光刻胶 | Fig. 3.11(b) |  |  |
|  | SiN HM 刻蚀 | 使用剩余间隔物图案刻蚀SiN HM | Fig. 3.11(b) | 干法刻蚀 |  |
|  | 垫氧化物去除 | 去除垫氧化物 | Fig. 3.11(c) | 湿法刻蚀 |  |
|  | 鳍片刻蚀 | 使用SiN HM图案刻蚀硅鳍片 | Fig. 3.11(c) | 干法刻蚀 |  |
| **4. 栅极形成 (Gate Last HKMG)** | ILD 沉积和CMP | 沉积ILD层，然后进行CMP | Fig. 3.12(a), (b) | CVD/CMP |  |
|  | SiN 和垫氧化物去除 | 去除SiN和垫氧化物 | Fig. 3.12(c) | 湿法刻蚀 |  |
|  | 牺牲氧化物生长 | 生长牺牲氧化物层 | Fig. 3.12(d) | 热氧化 |  |
|  | 离子注入 | 离子注入形成隔离井 | Fig. 3.12(d) | 离子注入 |  |
|  | 牺牲氧化物去除 | 去除牺牲氧化物 | Fig. 3.12(e) | 湿法刻蚀 |  |
|  | 虚拟栅极氧化物沉积 | 沉积虚拟栅极氧化物层 | Fig. 3.13(a) | ALD/CVD |  |
|  | 多晶硅沉积和CMP | 沉积多晶硅，然后进行CMP | Fig. 3.13(a) | CVD/CMP |  |
|  | 硬掩膜(HM)沉积和图案化 | 沉积HM层并进行图案化 | Fig. 3.13(b), (c) | ALD/CVD/光刻/刻蚀 |  |
|  | 多晶硅刻蚀 | 使用HM图案刻蚀多晶硅，形成虚拟多晶硅栅极 | Fig. 3.13(e) | 干法刻蚀 |  |
| **5. 源漏区(S/D) 形成** | 介电层沉积 | 沉积薄介电衬里层和厚的介电层 | Fig. 3.14(a) | ALD/CVD |  |
|  | PMOS/NMOS掩模和刻蚀 | 应用PMOS/NMOS掩模，刻蚀间隔物 | Fig. 3.14(b), (c) | 光刻/干法刻蚀 |  |
|  | 硅刻蚀和SiGe外延生长 | 硅刻蚀和SiGe外延生长 | Fig. 3.14(d) | 干法刻蚀/SEG |  |
| **6. 栅极替换和金属化 (Gate Last HKMG)** | ILD1 沉积和CMP | 沉积ILD1，然后进行CMP | Fig. 3.16(a), (b) | CVD/CMP |  |
|  | 虚拟多晶硅栅极去除 | 去除虚拟多晶硅栅极 | Fig. 3.16(c) | 湿法刻蚀 |  |
|  | 高k介电层沉积 | 沉积高k介电层 | Fig. 3.16(d) | ALD |  |
|  | TiN/TaN 沉积 | 沉积TiN和TaN | Fig. 3.16(d), (e) | ALD |  |
|  | NMOS掩模和刻蚀 | 应用NMOS掩模，刻蚀TaN和TiN | Fig. 3.17(a), (b) | 光刻/干法刻蚀 |  |
|  | TiAlN 沉积 | 沉积TiAlN | Fig. 3.17(c) | ALD |  |
|  | TiN 和W 沉积 | 沉积TiN和W | Fig. 3.17(d) | CVD |  |
|  | WCMP | 进行WCMP | Fig. 3.17(e) | CMP |  |
| **7. 后端工艺 (BEoL)** | ESL 沉积 | 沉积蚀刻停止层(ESL) |  | ALD/CVD |  |
|  | 金属层沉积和互连 | 沉积超低k介电层、帽氧化物层、TiN金属HM层、介电HM层和虚拟层，进行金属层沉积和互连 | Fig. 3.19 | 多种工艺 |  |


This should be a correctly formatted table.  Let me know if you have any further questions.
