# 有动作标签才加入动作损失 · DreamX

视频重建总是提供监督；机器人动作标签可加一条辅助流匹配损失。

x_tau=(1−tau)x+tau*epsilon，速度目标epsilon−x；有标签时视频/动作权重相同，无标签人类片段lambda=0。

继续拆：[2190小时不是全为人类视频](dx-data.md) · [动作标签对表征的贡献很小且非单向](dx-action-ablation.md)。

[本篇星系](../dreamx.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamx.md) · [原文依据](https://arxiv.org/pdf/2611.05377v1)
