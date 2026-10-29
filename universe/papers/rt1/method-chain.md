# 本篇方法链路 · RT-1

图像先经语言条件的 EfficientNet 提取特征，再由 TokenLearner 压成少量视觉 token；Transformer 融合短时历史并输出离散动作。动作同时覆盖机械臂、底盘和停止模式，策略以闭环方式反复读取图像。原文分别检验新指令、干扰物、新背景以及跨机器人数据混合的效果。

图像先经语言条件的 EfficientNet 提取特征，再由 TokenLearner 压成少量视觉 token；Transformer 融合短时历史并输出离散动作。动作同时覆盖机械臂、底盘和停止模式，策略以闭环方式反复读取图像。原文分别检验新指令、干扰物、新背景以及跨机器人数据混合的效果。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rt1-2212.06817/README.md#5-方法从六帧图像走到动作)

[本篇星系](../rt1.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/rt1-2212.06817/README.md) · [原文依据](https://www.roboticsproceedings.org/rss19/p025.html)
