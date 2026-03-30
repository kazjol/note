# 嵌入式底层知识专题索引

本目录用于承接 `chatgpt_window_questions_2026-03-30.md` 中整理出的知识主线，并将其进一步拆分为可独立阅读、可持续扩展的专题文档。

## 文档目标
- 将零散问题整理为专题化知识模块。
- 每篇文档都围绕“概念本质 → 运行机制 → 工程坑点 → 设计原因”展开。
- 便于后续继续追加案例、图示、代码片段与调试经验。

## 专题列表
1. [MMIO 与总线协议](./mmio_and_bus_protocols.md)
2. [RTOS 与上下文切换](./rtos_and_context_switch.md)
3. [链接脚本、启动流程与内存布局](./linker_startup_memory_layout.md)
4. [Linux 驱动模型与用户/内核边界](./linux_driver_model_and_kernel_user_boundary.md)
5. [IAP、Bootloader 与固件升级](./iap_bootloader_firmware_upgrade.md)
6. [Qi 协议与 ePWM](./qi_protocol_and_epwm.md)

## 推荐阅读顺序
1. 先看 **MMIO 与总线协议**，建立“代码如何碰到硬件”的基础认知。
2. 再看 **链接脚本、启动流程与内存布局**，理解程序如何真正启动并运行。
3. 接着看 **RTOS 与上下文切换**，理解并发、任务切换和同步。
4. 然后看 **Linux 驱动模型与用户/内核边界**，把 MCU 经验扩展到 Linux 系统层。
5. 再看 **IAP、Bootloader 与固件升级**，理解程序切换和在线升级的工程方案。
6. 最后看 **Qi 协议与 ePWM**，把前面建立的底层认知落到更具体的协议和控制应用。

## 后续扩展建议
后续可以继续新增这些专题：
- GPIO 与板级故障定位
- DMA、Cache 与一致性问题
- 中断架构与中断亲和性
- CAN / SPI / I2C 深度时序图解
- Linux 调度器与内存管理
- MCU 功耗管理与时钟树
