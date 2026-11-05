# 视频与动作共用条件而不互读 · DreamX

解码时视频流和动作流都读取query前缀，但彼此不注意。

query作为条件不读取其他token；Vt读Q0:t，Am读Q0:m。出现两种输出不等于它们通过直接注意力相互反馈。

继续拆：[有动作标签才加入动作损失](dx-loss.md)。

[本篇星系](../dreamx.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamx.md) · [原文依据](https://arxiv.org/pdf/2611.05377v1)
