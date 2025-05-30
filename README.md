# Universal Modular Power Electronics Building Blocks  
# 通用模块化电力电子套件

A modular power electronics hardware starter kit designed for sub-100V applications.  
Originally developed for the National Electronic Design Contest in 2021, now open-sourced for education and research.  
适用于低于 100V 场合的电力电子模块化套件，最初用于 2021 年全国大学生电子设计竞赛。

Based on Altium Designer  
基于Altium Designer

Refer to [DSPLibrary](https://github.com/BigdogManLuo/DSPLibrary) for the code and function libraries used during the contest.  
比赛中所使用的控制程序与封装函数库，请参阅：[DSPLibrary](https://github.com/BigdogManLuo/DSPLibrary)



## Features  
- **Modular design** 模块化结构  
  Independent control, sensing, and power stages  
  独立控制、传感、功率单元  

- **Standardized interface** 接口统一  
  All signals use consistent definitions and IDC-10 ribbon cable connections  
  全部采用一致接口信号定义，全部信号使用IDC-10排线连接  

- **Multiple adaptable configurations** 多种特性适配  
  Modules are designed to match different requirements such as low power, isolation, or high bandwidth  
  针对低功耗、隔离、高带宽等不同需求提供不同模块  



## Module Overview

| Module | Description 描述 |
|--------|------------------|
| `1.x`  | Synchronous buck converters (with different drivers) <br> 同步半桥模块（隔离 / 非隔离驱动） |
| `2.x`  | C2000-based control and expansion boards <br> C2000 控制器扩展与接口板 |
| `3.x`  | MSP430-based core board and regulators <br> MSP430 主控与扩展板 |
| `4.x`  | Auxiliary power modules: non-isolated, isolated, rectified <br> 各类辅助电源：非隔离、隔离、整流型 |
| `5.x`  | Current and voltage sensors (Hall-based or HF transformer) <br> 电流电压传感器模块（霍尔/高频CT） |
## Project File Structure
<pre>
.
├── 1.0 - SYNC_BUCK_Si8233_2023.4.21
├── 1.1 - SYNC_BUCK_IR2104_2021.7.31
├── 2.0 - DSP_Expansion_Board_for_28379D_LAUNCHXL
├── 2.1 - AD_EXPANSION_and_IO_Buffer_AHCT541_for_28379D_LAUNCHXL
├── 2.2 - AD_EXPANSION_for_28379D_LAUNCHXL
├── 2.3 - 28375D_Control_Card_2023.7.28
├── 3.0 - MSP430F5438_Core_Board
├── 3.1 - Expansion_Board_DCDC_Ver_for_MSP430
├── 3.2 - Expansion_Board_LDO_Ver_for_MSP430
├── 4.0 - Nonisolated_DCDC_3BUCK-1BOOST_AUX_Power
├── 4.1 - Isolated_AUX_Power_Board
├── 4.2 - Three_Phase_Diode_Rectifier_AUX_Power_Board
├── 4.3 - Auxiliary_Power_Board
├── 4.4 - SCT2430_TEST
├── 5.0 - Hall_Current_Sensor_LEM_55P
├── 5.1 - Hall_Voltage_Sensor
├── 5.2 - HF_Transducer_Voltage_Sensor
└── Electronic Design Contest Group 1.DsnWrk  ← Altium Project Workspace
</pre>


## Pin-out Defination 
![image](https://github.com/user-attachments/assets/fcaa4d5d-cc29-4079-bfd1-a378104c0f87)



## Disclaimer

This hardware is provided **as-is** for educational and experimental use only. The author assumes no responsibility for any injury, damage, or loss resulting from its use.

本项目仅供教学与实验用途。因使用本套件所引发的任何形式的人身伤害、设备损坏或其他损失，原作者概不承担责任。



## License

This project is licensed under the **BSD 3-Clause License** with additional restrictions.  
本项目遵循 **BSD 3-Clause License**，并附加以下使用限制：

**Additional Terms 附加条款：**  
This project is **not licensed for commercial use**.  
Sale, resale, or redistribution for profit is **prohibited without prior written permission** from the author.  
未经作者书面许可，禁止任何形式的商业用途、转售或盈利性再分发。

See [`LICENSE`](./LICENSE) for full details.  
完整内容请参见 [`LICENSE`](./LICENSE) 文件。



## Acknowledgments

Originally developed for the **National Electronic Design Contest 2021**.  
最初由参赛团队为 **2021 全国电子设计竞赛** 构建。

I extend my heartfelt appreciation to my teammates, [**Pu Chuanqing**](https://github.com/BigdogManLuo), 
and [**Xin Mingyuan**](https://github.com/Chen-JIANG-HHH), whose unwavering software support during the contest played a vital role in the success of this project.  
在此，谨向我的队友 [**濮川苘**](https://github.com/BigdogManLuo) 和 [**辛明远**](https://github.com/Chen-JIANG-HHH) 致以诚挚的感谢。

### ***Here’s to the alliance that saw us through it all.***
