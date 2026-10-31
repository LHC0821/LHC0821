<h1 align="center">👋 我是黎浩琛 · H+.</h1>

<p align="center">
  <strong>华南农业大学 · 电子信息工程（数字技术创新班）· 2025 级本科生</strong>
</p>

<p align="center">
  嵌入式开发 · 机器人电控 · 农业视觉<br>
  从感知、控制到执行，持续探索机器人系统的完整实现。
</p>

<p align="center">
  <img src="https://img.shields.io/badge/嵌入式开发STM32/ESP32/TI/C51-03234B?style=for-the-badge" alt="嵌入式开发" />
  <img src="https://img.shields.io/badge/机械Solidwork-CC0000?style=for-the-badge" alt="Solidwork" />
  <img src="https://img.shields.io/badge/ROS2-22314E?style=for-the-badge" alt="ROS2" />
  <img src="https://img.shields.io/badge/C/Python-00599C?style=for-the-badge" alt="C/Python" />
  <img src="https://img.shields.io/badge/嘉立创eda/AD-3776AB?style=for-the-badge" alt="嘉立创eda/AD" />
  <img src="https://img.shields.io/badge/视觉OpenCV/YOLO-5C3EE8?style=for-the-badge" alt="OpenCV/YOLO" />
</p>

<p align="center">
  <a href="https://github.com/LHC0821">GitHub：LHC0821</a> ·
  <a href="mailto:3060910239@qq.com">邮箱：3060910239@qq.com</a>
</p>

---

## 🧠 关于我

我主要使用 **C 和 Python**，围绕 **STM32、TI MSPM0、电机控制、板级硬件与农业视觉**开展项目实践。我关注机器人如何把感知结果转化为控制指令，再通过执行机构完成任务，希望逐步提升从硬件、固件到上位机应用的系统开发能力。

大一阶段，我在轮轨一体化底盘、电子设计竞赛和机械臂项目中积累了电控开发与系统联调经验，也承担过项目负责人、竞赛队长和技术组管理工作。做项目时，我重视软硬件配合、接口说明、调试记录与成果交付。

- **主要方向：** 嵌入式开发、机器人运动控制、农业视觉感知与系统集成。
- **当前实践：** 竞赛机器人开发、番茄目标检测与 RT-DETR 结构对比，以及校园学情分析系统探索。
- **科研与竞赛：** 参与 1 项大学生创新创业训练计划项目申请、2 项科研项目研究，并持续参加电子设计与机器人相关竞赛。
- **团队协作：** 性格开朗，愿意交流和分享，具有技术培训、任务分工与项目推进经验。

## 🛠️ 技术与实践

| 方向 | 技术与实践内容 |
| --- | --- |
| 嵌入式开发 | STM32F1、STM32H7、TI MSPM0、C51；C；HAL、DriverLib；中断、定时器、DMA 与外设驱动 |
| 通信与设备接入 | UART、I2C、SPI、CAN / FDCAN；电机通信、视觉数据收发、nRF24L01 无线通信 |
| 控制与运动 | PID、轮速闭环、数字量循迹、视觉误差控制、惯性测量与卡尔曼滤波；底盘和机械臂联调 |
| 机器人软件 | ROS2、MoveIt；双七轴机械臂运动规划及上下位机联调实践 |
| 视觉与实验 | Python、OpenCV、PyTorch / Ultralytics、RT-DETR；番茄检测数据处理、训练配置、结构对比与评估 |
| 硬件设计 | 嘉立创 EDA、Altium Designer；原理图与 PCB 设计、电源设计、通信与传感器接口集成；二至四层 PCB 设计实践 |
| 机械设计 | SolidWorks；机器人机构设计及软硬件协同调试 |
| 开发工具 | STM32CubeMX、CCS / SysConfig、VS Code Embedded IDE、Git；FreeRTOS 配置与示例学习 |
| 上位机与应用探索 | Java、JavaFX、WebSocket；轨迹处理与学情分析可视化 |

主要使用 **C、Python**；另有 **C++、Java、MATLAB** 的学习与使用经历。

---

## 🚀 代表项目

### 01 · 车载平衡球系统

**仓库：** [2026TI-match-ball-system](https://github.com/LHC0821/2026TI-match-ball-system)  
**个人分工：** 硬件、平衡球控制及机械；竞赛队长。  
**相关成果：** 2026 年电子设计竞赛 H 题 · 广东省二等奖。

面向电子设计竞赛车载滚球任务，参与滚球机构的设计、控制与整机协作。系统围绕 **STM32H723、BMI088 与 DM-4340 电机**，接收视觉端提供的球位偏差与速度，通过 CAN 通道控制摆杆。

- 负责硬件与机械相关工作，并承担平衡球控制任务。
- 控制方案结合视觉位置修正、球速项和加速度前馈，通过输出限幅与启动校准约束执行机构。
- 团队固件按 `app / service / device / platform` 分层组织，包含标称 500 Hz 控制调度、视觉通信、串口调参与状态日志。
- 仓库同时整理控制板、电源板及机械工程文件，便于回溯软硬件配合关系。

### 02 · 轮轨一体化底盘

**个人分工：** 大一上学期任电控负责人，大一下学期任项目负责人。

- 基于 **STM32H723 与 CAN / FDCAN** 参与多节点电机通信及底盘电控开发。
- 围绕舵轮驱动开展协同运动控制、运动学解算、零位调试与整机联调。
- 参与电源系统、PCB 与信号集线板设计，结合供电、信号连接和执行机构需求推进软硬件配合。
- 在项目负责人阶段承担任务协调与项目推进工作，积累软硬件一体化系统开发经验。

### 03 · Longinus 竞赛机器人

**仓库：** [Competition-Robot-2026-Longinus](https://github.com/LHC0821/Competition-Robot-2026-Longinus)  
**个人分工：** 末端控制与视觉相关开发。

- 围绕机器人末端执行与视觉功能参与开发，关注感知结果与执行动作之间的配合。
- 参与团队电控工程协作，开展相关模块开发与系统联调。
- 当前个人仓库公开快照主要展示 **STM32H723 四舵轮底盘与公共电控模块的集成基线**；末端与视觉部分随实际进展补充展示。

### 04 · 番茄目标检测与 RT-DETR 结构对比

**仓库：** [RTDETR-main](https://github.com/LHC0821/RTDETR-main)  
**个人分工：** 项目负责人；负责数据集、训练配置、结构对比及优化实验。

基于现有 **RT-DETR / Ultralytics** 实现，面向番茄农业场景开展目标检测应用研究。

- 配置 `ripe / stem / unripe` 三类检测任务，处理数据划分与标注格式转换。
- 围绕 **HAFB、SimAM、P2 细节分支、CGAFusion** 等已有模块开展组合配置与结构对比。
- 关注细小果梗与果实的检测表现，以及检测精度和计算开销之间的取舍。
- 使用训练、验证与分析脚本记录和比较实验，持续完善基线、消融实验及可复现实验材料。

### 05 · 模块化八路循迹控制

**仓库：** [LineFollow_Modular](https://github.com/LHC0821/LineFollow_Modular)

将电赛循迹代码整理为 `app / service / domain / platform` 分层结构，保留旧接口兼容方式与 MSPM0 接入示例。

- 对八路二值输入进行位置估计与平滑，以比例转向生成左右轮目标速度，再接入已有速度 PID。
- 包含起步斜坡、停车标记确认、丢线超时、停止锁存和参数校验。
- 提供行为测试、验证记录、兼容工程与分层工程，便于对照原行为并进行后续移植。

### 06 · TI 外设模块与视觉云台实践

**仓库：** [Ti-Prepare](https://github.com/LHC0821/Ti-Prepare) · [JC 视觉云台](https://github.com/LHC0821/JC-Brushless-Actuation-for-Gimbal-Stabilization)

- 整理 **TI MSPM0** 平台的 OLED、按键、电机、编码器、PID、循迹、日志及无线通信模块。
- 使用 **nRF24L01** 开展双节点通信开发，提供文本、整数与二进制数据接口。
- 在 **STM32F103** 云台原型中编写视觉数据接收、协议解析和双轴误差调节逻辑，探索视觉反馈与执行机构控制的配合。

### 07 · STM32F103RCT6 多接口控制板

**仓库：** [stm32f103rct6-core-board](https://github.com/LHC0821/stm32f103rct6-core-board)

- 使用 **嘉立创 EDA 专业版**整理原理图与 PCB 工程。
- 集成电源管理、CAN、RS485、UART、I2C、SPI、TB6612 电机驱动、PWM 及传感器接口。
- 已公开设计工程与设计说明，后续继续推进板级验证。

### 08 · 校园学情分析系统

围绕轨迹数据处理与学习行为分析开展系统探索。

- 基于轨迹数据进行学习行为建模，使用 **卡尔曼滤波**优化轨迹。
- 基于 **WebSocket** 探索实时数据通信。
- 使用 **JavaFX** 开展上位机界面与可视化开发。

## 🤖 其他机器人项目经历

| 项目 | 参与内容 |
| --- | --- |
| 双七轴达妙机械臂 | 使用 ROS2、MoveIt 参与运动规划、控制与上下位机联调，涉及机器人运动学和控制算法应用 |
| 茶叶机械臂 | 参与末端实现、单片机控制、硬件联调与机构控制验证 |

---

## 🏆 竞赛与荣誉

| 成果 | 角色 |
| --- | --- |
| 2026 年电子设计竞赛 H 题 · 广东省二等奖 | 队长 |
| 单片机协会第十六届智能小车竞赛 · 二等奖 | 队长 |
| 校科联极客挑战赛 · 二等奖 | 项目负责人 |
| 光电信息协会光电赛入门组 · 三等奖 | 队长 |
| 校级一等奖学金 | 获得者 |

## 🏫 教育与组织经历

### 华南农业大学

**电子信息工程（数字技术创新班）｜2025 级本科生**

担任电信创新班班长，曾任学习委员、临时班长。

### 第 18 届单片机协会 · 培训部部长

- 参与嵌入式开发学习与实践，开展基础外设驱动和控制系统开发。
- 围绕 STM32 / C51 积累实战经验，并参与技术培训与交流。

### 第 16 届校科联 · 自科部电子方向正部长

- 参与电子设计相关项目，开展电路设计、调试及系统联调。
- 在项目实践中积累硬件设计、底盘运动学解算与团队协作经验。

### 第 5 届 Agrotech 智能机械协会 · 电控组组长、机械臂运控组副组长

- 参与机械臂控制系统开发，基于 ROS2 + MoveIt 开展运动规划与控制实践。
- 参与电控与运控相关任务协调，推动模块开发及软硬件联调。

这些经历让我逐步形成了从任务拆分、接口沟通到联调交付的项目推进习惯，也让我更重视技术分享和团队协作。

---

## 📂 仓库导航

| 仓库 | 内容 |
| --- | --- |
| [2026TI-match-ball-system](https://github.com/LHC0821/2026TI-match-ball-system) | 电赛车载平衡球固件、硬件与机械资料 |
| [Competition-Robot-2026-Longinus](https://github.com/LHC0821/Competition-Robot-2026-Longinus) | 竞赛机器人团队工程，公开基线以底盘为主 |
| [RTDETR-main](https://github.com/LHC0821/RTDETR-main) | 番茄目标检测训练与结构配置实验 |
| [LineFollow_Modular](https://github.com/LHC0821/LineFollow_Modular) | 八路数字量循迹解耦、移植与行为测试 |
| [Ti-Prepare](https://github.com/LHC0821/Ti-Prepare) | TI 备赛外设驱动与应用模块 |
| [JC-Brushless-Actuation-for-Gimbal-Stabilization](https://github.com/LHC0821/JC-Brushless-Actuation-for-Gimbal-Stabilization) | JC 电机与视觉云台控制原型 |
| [stm32f103rct6-core-board](https://github.com/LHC0821/stm32f103rct6-core-board) | STM32 多接口控制板硬件工程 |
| [LHC0821](https://github.com/LHC0821/LHC0821) | 个人主页与项目索引 |

## 🌱 下一阶段

我希望在农业机器人相关实验室、竞赛与科研项目中继续学习，重点深入：

- **运动控制：** 完善电机与机器人控制中的零位标定、反馈处理及异常工况验证。
- **农业视觉：** 深入小目标检测，补全基线、消融实验和误检漏检分析。
- **系统集成：** 推进视觉与末端执行的协作，将单个模块沉淀为可复现的系统成果。
- **开发能力：** 在嵌入式与机器人实践基础上，逐步拓展上位机、应用开发与全栈能力。

## 📫 联系我

- **GitHub：** [LHC0821](https://github.com/LHC0821)
- **邮箱：** [3060910239@qq.com](mailto:3060910239@qq.com)

欢迎交流嵌入式开发、机器人电控与农业视觉相关问题，也期待在实验室、竞赛和科研项目中与更多伙伴合作。

<p align="center"><sub>更新于 2026 年 10 月 31 日</sub></p>
