# 联合预测损失 · MuZero

策略、价值、奖励误差共同更新h/g/f。

k0只有p/v，k1…K再加r；加L2正则。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/muzero-1911.08265/README.md#36-损失函数三份作业一起改hgf)

继续拆：[软分布交叉熵](ce.md) · [展开梯度缩放](grad.md)。

[本篇星系](../muzero.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/muzero-1911.08265/README.md) · [原文依据](https://arxiv.org/pdf/1911.08265v2)
