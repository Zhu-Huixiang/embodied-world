# 把去视频部署路径也练到 · TAPESTRY

训练时单独练动作分支，部署才能删除未来视频。

固定5epoch仅联合训练的模型在推理生成视频时达到78%，改为动作独立推理会失败；不能训练时依赖视频、部署时直接删掉。

继续拆：[零末端SNR下的一步DDIM](one-step.md)。

[本篇星系](../tapestry.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/tapestry.md) · [原文依据](https://arxiv.org/pdf/2610.36823v1)
