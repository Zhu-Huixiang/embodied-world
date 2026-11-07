# 会控制之后，视觉该接在哪里？ · Latent RL Prior

特权状态训练出的控制能力，需要从图像建立可部署的条件入口。

本文保留动作生成与本体处理，仅替换任务条件来源，检验少量下游视觉示范能否接入已有RL先验。

继续拆：[两份数据不要求轨迹配对](lrp-two-datasets.md) · [冻结decoder并保留本体条件路径](lrp-freeze.md) · [三任务均为同本体仿真](lrp-tasks.md) · [冻结先验也会冻结能力边界](lrp-boundaries.md)。

[本篇星系](../latent-rl-prior.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/latent-rl-prior.md) · [原文依据](https://arxiv.org/pdf/2611.08458v1)
