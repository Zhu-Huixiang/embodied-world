# 公共probe测表示，不是闭环成功率 · DreamX

冻结所有表示，用相同attentive probe完成动作回归和分类。

每token投影768维后池化；视频方法用元数据恢复中间帧并保留各自支持的时窗。相同probe并不代表预训练数据、backbone或上下文完全相同。

继续拆：[表征误差与语义分类同时改善](dx-lary-results.md)。

[本篇星系](../dreamx.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamx.md) · [原文依据](https://arxiv.org/pdf/2611.05377v1)
