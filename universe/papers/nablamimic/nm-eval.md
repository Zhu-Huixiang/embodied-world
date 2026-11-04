# 整片段归一化回报评测 · ∇Mimic

每条动作从第一帧确定性执行一次，跌倒后的剩余回报归零。

40条等权平均、无观测噪声/随机化；评测在MuJoCo Warp。同训练库覆盖检验不同于未见动作泛化与实机迁移。

继续拆：[v1三seed训练效率](nm-results.md)。

[本篇星系](../nablamimic.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/nablamimic.md) · [原文依据](https://arxiv.org/pdf/2610.41654v1)
