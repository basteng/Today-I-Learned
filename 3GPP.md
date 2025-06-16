- [Perplexity](#perplexity)
  - [3GPP TS23.122与TS31.102技术解析](#3gpp-ts23122与ts31102技术解析)
    - [一、SIM/USIM卡文件系统结构（TS31.102）](#一simusim卡文件系统结构ts31102)
    - [二、PLMN选择与注册机制（TS23.122）](#二plmn选择与注册机制ts23122)
- [GPT](#gpt)
  - [一、3GPP TS 23.122：PLMN选择与注册（PLMN Selection）](#一3gpp-ts-23122plmn选择与注册plmn-selection)
    - [1. 概述](#1-概述)
    - [2. PLMN选择类型](#2-plmn选择类型)
    - [3. 注册过程简化流程：](#3-注册过程简化流程)
    - [4. PLMN优先级来源](#4-plmn优先级来源)
  - [二、3GPP TS 31.102：USIM 文件结构（USIM File Structure）](#二3gpp-ts-31102usim-文件结构usim-file-structure)
    - [1. 文件系统基本结构（TLV格式）](#1-文件系统基本结构tlv格式)
  - [三、常见相关文件（EFs）介绍](#三常见相关文件efs介绍)
  - [四、PLMN ID 格式说明](#四plmn-id-格式说明)
  - [五、卡文件如何参与PLMN选择](#五卡文件如何参与plmn选择)
  - [六、补充说明：Roaming 和 PLMN黑名单](#六补充说明roaming-和-plmn黑名单)
- [豆包](#豆包)
    - [3GPP TS23.122与TS31.102概述](#3gpp-ts23122与ts31102概述)
    - [卡文件及其存储结构](#卡文件及其存储结构)
    - [PLMN选择和注册](#plmn选择和注册)

# Perplexity

## 3GPP TS23.122与TS31.102技术解析

### 一、SIM/USIM卡文件系统结构（TS31.102）

**文件系统架构**  
采用树状层级结构，包含以下核心组件：  
- **MF（主文件）**：根目录，存储全局信息如ICCID（3F00）[1][6]  
- **DF（专用文件）**：二级目录，如：  
  - **DFTELECOM（7F10）**：存储通信相关数据  
  - **DFGSM（7F20）**：存储GSM网络参数[1][10]  
- **EF（基本文件）**：数据存储单元，主要类型包括：  

| 文件类型       | 结构特性                 | 典型示例                 |
|----------------|--------------------------|--------------------------|
| 透明文件       | 连续字节流               | EFIMSI（6F07）           |
| 线性定长文件   | 固定长度记录             | EFLOCI（位置信息）        |
| 循环文件       | 覆盖最旧记录             | EFSMS（短信存储）        |

**关键存储内容**：  
1. **EFPLMN**（6F30）  
   - 存储禁止PLMN列表（Forbidden PLMNs）  
   - 记录格式：MCC+MNC（3字节）[6][7]  
2. **EFEHPLMN**（6F50）  
   - 等效HPLMN列表，优先级高于IMSI衍生HPLMN[4][8]  
3. **EFLOCI**（6F7E）  
   - 位置区域标识（LAI/TAC）及更新状态[5][7]  

### 二、PLMN选择与注册机制（TS23.122）

**选择模式**  
1. **自动模式**  
   - 优先级顺序：  
     ```
     1. EHPLMN/HPLMN → 2. 用户预设PLMN → 3. 运营商预设PLMN  
     → 4. 高信号质量PLMN → 5. 其他PLMN[14][16]
     ```
   - 信号质量评估标准：  
     - GERAN：RxLev ≥ -85dBm  
     - NR：SS-RSRP ≥ -110dBm[2][9]  

2. **手动模式**  
   - 用户从扫描列表中选择PLMN  
   - 失败后进入"No Service"状态[4][11]  

**注册流程**  
1. **成功注册条件**：  
   - 驻留合适小区（Suitable Cell）  
   - 完成位置注册（LR）流程[4][9]  
2. **状态机转换**：  
   - 空闲态 → 尝试注册 → 正常服务态/受限服务态  
3. **异常处理**：  
   - 收到#15拒绝原因码时，将LA/TA加入禁止列表[3][12]  
   - 周期性HPLMN搜索间隔：6分钟（默认值）[4][8]  

**关键技术特性**  
- **等效PLMN**：允许跨运营商共享核心网时保持服务连续性[4][8]  
- **Steering of Roaming**：通过EFSoR-CMCI实现网络切换控制[13]  
- **5G增强**：支持SUCI加密计算和eDRX节能参数配置[13][5]  

该技术体系通过标准化文件结构和网络选择算法，确保了跨厂商设备的互操作性和漫游服务的可靠性。最新规范已支持5G NSA/SA架构下的增强功能，包括网络切片关联和卫星网络接入控制[13][1]。

[1] https://python.quectel.com/doc/quecpython/Application_guide/en/network-comm/sim/SIM-card-file-system.html
[2] https://www.arib.or.jp/english/html/overview/doc/STD-T63v11_00/5_Appendix/Rel12/23/23122-c60.pdf
[3] https://www.etsi.org/deliver/etsi_ts/123100_123199/123122/14.04.00_60/ts_123122v140400p.pdf
[4] https://www.tech-invite.com/3m23/toc/tinv-3gpp-23-122_f.html
[5] https://www.etsi.org/deliver/etsi_ts/131100_131199/131102/15.08.00_60/ts_131102v150800p.pdf
[6] https://www.arib.or.jp/english/html/overview/doc/STD-T63v9_60/5_Appendix/Rel6/31/31102-6n0.pdf
[7] https://www.3gpp.org/ftp/tsg_t/WG3_USIM/TSGT3_01/docs/t3-99032.pdf
[8] https://www.arib.or.jp/english/html/overview/doc/STD-T63V12_30/5_Appendix/Rel13/22/22011-d60.pdf
[9] https://www.3gpp.org/DynaReport/31-series.htm
[10] https://cedric.cnam.fr/~bouzefra/cours/CartesSIM_Fichiers_Anglais.pdf
[11] https://www.arib.or.jp/english/html/overview/doc/STD-T63V12_10/5_Appendix/Rel9/22/22011-940.pdf
[12] https://www.arib.or.jp/english/html/overview/doc/STD-T63v9_10/5_Appendix/Rel7/23/23122-7c1.pdf
[13] https://trustedconnectivityalliance.org/wp-content/uploads/2023/05/TCA_Recommended-5G-SIM-_FINAL.pdf
[14] https://www.3gpp.org/dynareport/23122.htm
[15] https://www.arib.or.jp/english/html/overview/doc/STD-T63v10_70/5_Appendix/Rel11/31/31101-b10.pdf
[16] https://www.arib.or.jp/english/html/overview/doc/STD-T63v9_60/5_Appendix/Rel5/23/23122-530.pdf
[17] https://www.arib.or.jp/english/html/overview/doc/STD-T63v11_00/5_Appendix/Rel12/22/22011-c20.pdf
[18] https://www.etsi.org/deliver/etsi_ts/123100_123199/123122/16.07.00_60/ts_123122v160700p.pdf
[19] https://www.etsi.org/deliver/etsi_ts/131100_131199/131102/11.06.00_60/ts_131102v110600p.pdf
[20] https://www.etsi.org/deliver/etsi_ts/123100_123199/123122/15.06.00_60/ts_123122v150600p.pdf
[21] https://cdn.standards.iteh.ai/samples/51689/6d70bcc9eef1454db157b371a99ee586/ETSI-TS-123-122-V14-2-0-2017-04-.pdf
[22] https://www.arib.or.jp/english/html/overview/doc/STD-T63V9_21/2_T63/ARIB-STD-T63/Rel5/31/A31102-5e0.pdf
[23] https://www.3gpp.org/ftp/tsg_ct/WG1_mm-cc-sm_ex-CN1/TSGC1_143_Goteborg/Draft%20Specifications/Uploaded%20on%2022nd%20June%202023/23122-i30_rm.docx
[24] https://www.3gpp.org/dynareport/31102.htm
[25] ftp://www.3gpp.org/TSG_T/TSG_T/TSGT_05/Docs/PDFs/TP-99186.pdf
[26] http://www.arib.or.jp/english/html/overview/doc/STD-T63V12_20/5_Appendix/Rel13/31/31116-d00.pdf
[27] https://www.etsi.org/deliver/etsi_ts/123100_123199/123122/15.04.00_60/ts_123122v150400p.pdf
[28] https://cdn.standards.iteh.ai/samples/64542/88d01a82d98746a49ec882d04679b2c6/ETSI-TS-123-122-V17-6-0-2022-05-.pdf

# GPT

你提到的内容非常专业，涉及**3GPP TS 23.122** 和 **TS 31.102** 这两个规范文件，主要关系到**USIM卡文件结构**、**PLMN选择和注册过程**。下面我为你分部分详细整理讲解：

---

## 一、3GPP TS 23.122：PLMN选择与注册（PLMN Selection）

### 1. 概述

TS 23.122 定义了\*\*公共陆地移动网络（PLMN）\*\*的选择与注册流程，是移动终端（UE）接入网络的核心机制。

### 2. PLMN选择类型

* **自动模式（Automatic mode）**：UE优先选择\*\*用户偏好列表（User Preferred PLMN list）\*\*中的PLMN。
* **手动模式（Manual mode）**：用户从可用网络中手动选择。

### 3. 注册过程简化流程：

```text
[1] UE 启动 -> 读取USIM卡中的PLMN优先列表
[2] 搜索所有广播PLMN（扫描频段）
[3] 与优先PLMN进行连接尝试
[4] 如果成功，发送注册请求 (Tracking Area Update / Attach Request)
[5] 网络接受并分配临时ID（如GUTI），完成注册
```

### 4. PLMN优先级来源

* SIM卡中 `EFPLMNwAcT`：优先注册PLMN及其接入技术（如UTRAN、E-UTRAN等）
* SIM卡中 `EFHPLMN`：归属网络优先级间隔时间
* ME（移动设备）自身设定的优先级列表

---

## 二、3GPP TS 31.102：USIM 文件结构（USIM File Structure）

TS 31.102 是对 **USIM卡的逻辑结构** 和**文件系统**的标准定义。

### 1. 文件系统基本结构（TLV格式）

USIM卡采用**文件系统树状结构**，包含：

* **MF（Master File）**：主目录，唯一
* **DF（Dedicated File）**：目录文件
* **EF（Elementary File）**：基本文件，存储数据

```
MF
 ├── DF-GSM
 │     ├── EFPLMNsel
 │     ├── EFLOCI
 │     ├── EFAD
 │     └── ...
 ├── DF-UMTS (或DF-USIM)
 │     ├── EFIMSI
 │     ├── EFARR
 │     ├── EFPHPLMN
 │     └── ...
```

---

## 三、常见相关文件（EFs）介绍

| 文件名             | 内容描述                                              | 文件ID (hex) |
| --------------- | ------------------------------------------------- | ---------- |
| **EFIMSI**      | 用户的IMSI（International Mobile Subscriber Identity） | `6F07`     |
| **EFPLMNsel**   | 优选PLMN列表（Preferred PLMN List）                     | `6F30`     |
| **EFHPLMN**     | 高优先级PLMN列表（High Priority PLMN）                    | `6F31`     |
| **EFOPLMNwACT** | 禁止PLMN列表（Operator Controlled PLMN）                | `6F61`     |
| **EFLOCI**      | 上次注册的LAC、TMSI、PLMN ID                             | `6F7E`     |
| **EFAD**        | 位置更新参数、MNC长度等                                     | `6FAD`     |
| **EFARR**       | 访问规则（用于文件访问权限控制）                                  | `6F06`     |

---

## 四、PLMN ID 格式说明

* PLMN = MCC + MNC

  * MCC（三位）：Mobile Country Code，如中国是 460
  * MNC（二或三位）：Mobile Network Code，如中国移动是 00、02等
* 举例：中国移动 PLMN = 46000

---

## 五、卡文件如何参与PLMN选择

1. **读取EFPLMNsel**

   * UE从卡中读取优选PLMN（包含接入技术）
   * 每条记录由 PLMN + Access Tech (GERAN, UTRAN, E-UTRAN等) 组成
2. **根据PLMN优先级排序尝试注册**
3. **失败时查找其他PLMN（广播表）**
4. **记录成功注册的PLMN到EFLOCI（包含PLMN ID + LAC）**

---

## 六、补充说明：Roaming 和 PLMN黑名单

* EFOPLMNwACT：由运营商配置，指定**禁止漫游**的PLMN列表
* EFFPLMN：Frequent PLMN，UE可记录最近成功接入的网络，用于快速切换

---

如你需要查看具体3GPP文档的哪一节、或进一步解释某个EF文件的编码格式（如TLV结构、字节意义等），我可以继续为你详细拆解。是否需要举一个 PLMN选择的流程代码或EFPLMNsel文件解码示例？

# 豆包

以下是关于3GPP TS23.122、31.102中卡文件及其存储结构、PLMN选择和注册的相关内容：

### 3GPP TS23.122与TS31.102概述
- **TS23.122**：主要涉及到公共陆地移动网络（PLMN）的选择和重选相关的流程、策略以及参数等内容，对UE（用户设备）如何选择合适的PLMN网络进行了规范。
- **TS31.102**：定义了USIM（通用用户识别模块）卡的文件结构、内容以及相关的操作等，包括卡中存储的各种文件以及这些文件的作用和访问方式等。

### 卡文件及其存储结构
- **文件类型**：在TS31.102中规定，USIM卡中的文件以树形结构存储。例如，EFUST（USIM Service Table）文件指示哪些服务可用；EFNSI（Network Specific Identifier）文件包含以NAI格式的网络特定标识符作为SUPI；还有EF5GS3GPPNSC（5GS 3GPP Access NAS Security Context）存储NAS层安全相关的K和count值等。
- **存储结构**：USIM卡文件系统采用分层的树形结构，类似于计算机中的文件系统。最顶层是主文件（MF），从主文件可以向下分支到不同的专用文件（DF），再从专用文件可以进一步找到基本文件（EF）。这种结构使得不同类型的信息能够被清晰地组织和管理，便于UE和网络对卡内信息的读取和使用。

### PLMN选择和注册
- **PLMN选择**：UE开机后，在SIM卡初始化还未完成前，会先尝试获取限制服务，以便支持拨打紧急电话。SIM卡初始化完成后，UE会进行PLMN选择。其顺序一般为RPLMN（Registered PLMN，已注册的PLMN）＞EHPLMN（Equivalent Home PLMN，等效归属PLMN）＞EPLMN/HPLMN（Visited PLMN或Home PLMN，拜访PLMN或归属PLMN）＞UPLMN（User Controlled PLMN，用户控制的PLMN）＞OPLMN（Operator Controlled PLMN，运营商控制的PLMN）。UE通过扫描不同的频点，获取小区的系统消息，从中解析出PLMN相关信息，判断是否是合适的PLMN。
- **注册流程**：UE选择好PLMN后，会向该PLMN网络发起注册请求。如果UE处于CM - IDLE状态，(R)AN会将注册请求消息包含在Initial UE消息中发送给初始AMF；如果UE处于CM - CONNECTED状态并触发注册过程，NG - RAN会在上行NAS传输消息中将注册请求消息发送给服务AMF。AMF收到注册请求后，可能会根据UE的SUPI、订阅信息等决定是否将注册请求重新路由到另一个AMF。注册过程中还涉及到安全认证等流程，以确保UE和网络之间的通信安全。只有通过一系列的验证和流程后，UE才能成功注册到PLMN网络，从而获得网络提供的各种服务。