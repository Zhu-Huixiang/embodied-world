# 能线性读出力，不等于显式力控制 · Latent RL Prior

单独force-annotated probe数据上，冻结策略并拟合decoder各层的ridge线性探针。

四类目标为总抓握法向力、逐指法向、逐指切向、逐指笛卡尔力；L1–L8，单位N/RMSE，3policy seed平均，同IID probe test episodes；较低RMSE说明表征可读性，未施加因果干预。

[本篇星系](../latent-rl-prior.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/latent-rl-prior.md) · [原文依据](https://arxiv.org/pdf/2611.08458v1)
