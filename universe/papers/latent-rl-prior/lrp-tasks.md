# 三任务均为同本体仿真 · Latent RL Prior

MuJoCo Warp中KUKA iiwa配SHARPA手，分别测试刷子对齐、抬门和双臂装配。

刷子未见于预训练但属于同类姿态对齐；抬门与双臂为新任务。双臂仍用同一arm–hand系统，不构成跨机器人形态迁移。

继续拆：[对齐成功不是十步连续达标](lrp-criterion.md) · [少量示范仍来自另训的RL策略](lrp-demonstrations.md) · [比较的是示范预算，不是相同训练预算](lrp-protocol.md) · [训练时不见的新质量检验](lrp-mass.md) · [能线性读出力，不等于显式力控制](lrp-force-probe.md)。

[本篇星系](../latent-rl-prior.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/latent-rl-prior.md) · [原文依据](https://arxiv.org/pdf/2611.08458v1)
