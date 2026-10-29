# 右移目标与teacher forcing · Transformer

用已知真实前缀训练下一token预测。

训练喂入右移目标，不等于生成时可看到未产生真值；运行仍逐token推进。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md#5-训练答案右移未来遮住)

继续拆：[标签平滑](smoothing.md) · [预热后衰减学习率](warmup.md)。

[本篇星系](../attention.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md) · [原文依据](https://arxiv.org/abs/1706.03762v7)
