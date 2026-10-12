# 本篇方法链路 · EfficientZero

编码器把图像变成潜状态，动力学网络预测下一潜状态，MCTS 在这个模型里比较动作。EfficientZero 用预测潜状态与真实下一帧编码的一致性补强动力学监督，预测累计价值前缀，并重分析旧数据来缓解离策略目标偏差。它测试的是有限交互预算下的游戏与模拟控制效率。

编码器把图像变成潜状态，动力学网络预测下一潜状态，MCTS 在这个模型里比较动作。EfficientZero 用预测潜状态与真实下一帧编码的一致性补强动力学监督，预测累计价值前缀，并重分析旧数据来缓解离策略目标偏差。它测试的是有限交互预算下的游戏与模拟控制效率。

[本篇星系](../efficientzero.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/efficientzero.md) · [原文依据](https://proceedings.neurips.cc/paper/2021/hash/d5eca8dc3820cad9fe56a3bafda65ca1-Abstract.html)
