# 本篇方法链路 · CLIPort

语义支路用 CLIP 提取 RGB 与指令概念，空间支路从 RGB-D 学习保持位置结构的特征；两路信息进入 Transporter 的拾取与放置预测。拾取位置先决定裁出哪块特征，再用互相关找到合适的放置区域。原文在多任务仿真和真实桌面上检验新物体、语义概念与少量示范。

语义支路用 CLIP 提取 RGB 与指令概念，空间支路从 RGB-D 学习保持位置结构的特征；两路信息进入 Transporter 的拾取与放置预测。拾取位置先决定裁出哪块特征，再用互相关找到合适的放置区域。原文在多任务仿真和真实桌面上检验新物体、语义概念与少量示范。

[本篇星系](../cliport.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/cliport.md) · [原文依据](https://proceedings.mlr.press/v164/shridhar22a.html)
