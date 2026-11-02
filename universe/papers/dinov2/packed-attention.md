# 打包序列却隔开注意力 · DINOv2

将长短裁切序列合并处理，用块对角mask阻止不同序列相互读取。

这种打包改变计算组织，保持每个序列独立前向的结果；它不是让同batch所有图共享内容。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#51-计算工程怎样改变可训练规模)

继续拆：[被丢弃分支不再白算](stochastic-depth.md) · [分片训练状态](fsdp.md)。

[本篇星系](../dinov2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md) · [原文依据](https://arxiv.org/pdf/2304.07193v2)
