# GAE把回报变为相对优势 · DeepMimic

用λ-return减当前value，得到动作相对该状态平均表现的优势。

它同时依赖实际奖励和critic，区别于直接模仿参考动作标签。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/deepmimic-1804.02717/README.md#4-背景奖励怎样改掉下一次动作)

[本篇星系](../deepmimic.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/deepmimic-1804.02717/README.md) · [原文依据](https://xbpeng.github.io/projects/DeepMimic/DeepMimic_2018.pdf)
