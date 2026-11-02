# 被丢弃分支不再白算 · DINOv2

高随机深度时真正跳过丢弃残差的计算，而非算完再乘零。

从头训练drop-rate0.4；实施中随机打乱batch并选取参与该块计算的样本，节省对应计算与内存。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#51-计算工程怎样改变可训练规模)

[本篇星系](../dinov2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md) · [原文依据](https://arxiv.org/pdf/2304.07193v2)
