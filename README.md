# embedded-learning-notes · 我的嵌入式学习可视化笔记

把"看不见的机制"画出来 —— 一批用图形和动画讲嵌入式与 C 语言底层概念的学习笔记。

> **这是早期学习笔记，不是教程。** 我还在学，图里的术语、箭头方向、类比都可能有不准确甚至错的地方。
> 如果你发现错了，欢迎开 issue 告诉我 —— 那对我是真帮助。

## 为什么做这批图

我是机械背景，转过来学嵌入式和 C 语言。看书时最难受的不是公式，而是**看不见**：

- 电流怎么从引脚流到 LED？
- 指针到底"指"在哪儿？
- CPU 一个指令周期里，取指、译码、执行到底谁先谁后？

文字讲三遍我还是没画面，于是干脆把它们**画出来、动起来**。做法是和一个 AI 助手配合：我出理解与判断，它帮我把图/动画生成出来，我再逐张核对哪里画错了。

## 内容

| 主题 | 文件 | 讲什么 | 形式 |
|---|---|---|---|
| **GPIO 点灯** | [gpio/gpio-led-infographic.png](gpio/gpio-led-infographic.png) | 从供电、时钟、寄存器到推挽输出、限流电阻、LED 的完整链路 | 信息图 |
| | [gpio/gpio-led-comic.png](gpio/gpio-led-comic.png) | 同一件事的漫画版（为什么"写个 1 灯就亮") | 漫画 |
| **MCU 架构** | [mcu/mcu-classic-architecture.png](mcu/mcu-classic-architecture.png) | 经典 MCU 架构：内核 / 总线 / 外设 / 存储器怎么连 | 架构图 |
| | [mcu/mcu-classic-architecture.html](mcu/mcu-classic-architecture.html) | 同上，可交互版本（浏览器直接打开） | 交互页 |
| | [mcu/mcu-c-cpu-interactive.html](mcu/mcu-c-cpu-interactive.html) | C 语言、CPU、MCU 三者关系 | 交互页 |
| | [mcu/mcu-c-cpu-relations.mp4](mcu/mcu-c-cpu-relations.mp4) | 同上，动画短片 | 视频 |
| **存储器** | [memory/memory-three-compared.png](memory/memory-three-compared.png) | Flash / SRAM / 寄存器 三大件对比 | 对比图 |
| **CPU 执行** | [cpu/cpu-fetch-decode-execute.html](cpu/cpu-fetch-decode-execute.html) | 取指 → 译码 → 执行 一个指令周期动画 | 动画 |
| **FOC 控制** | [foc/foc-coordinate-transform.html](foc/foc-coordinate-transform.html) | Clarke / Park 坐标变换（电机矢量控制） | 动画 |
| | [foc/foc-control-block.png](foc/foc-control-block.png) | FOC 控制框图 | 框图 |

`.html` 文件是零依赖的（原生 Canvas/SVG），**双击即在浏览器里跑**，不用装任何东西。

## 怎么用

- 想快速看图：点上面表格里的链接
- 想动手玩：把 `.html` 下载下来直接在浏览器打开
- 想照着做同样的图：这套流程本身是可复用的 —— 先自己读懂，再让 AI 按你的理解画，最后核对

## 许可

自由取用、修改、转载（注明来源即可）。里面若有错，**以权威教材和数据手册为准**，别以我为标准。
