# 冻结的未来表征教师 · DreamFree

教师从当前与未来视频得到监督目标。

教师保持双向视频注意力和各帧文本交叉注意力；用固定噪声水平扰动真实视频后取隐藏层未来token，训练中不更新。

继续拆：[教师固定噪声水平](df-noise.md) · [从当前token扩展未来token](df-projector.md)。

[本篇星系](../dreamfree.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamfree.md) · [原文依据](https://arxiv.org/pdf/2611.04527v1)
