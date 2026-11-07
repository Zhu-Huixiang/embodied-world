# PPO的有方向裁剪 · DeepMimic

新旧动作概率比与优势相乘，并和裁剪项取min。

正优势封顶过度增大概率的收益，负优势封顶过度减小概率的收益；越界并非总梯度都零。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/deepmimic-1804.02717/README.md#4-背景奖励怎样改掉下一次动作)

[本篇星系](../deepmimic.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/deepmimic-1804.02717/README.md) · [原文依据](https://xbpeng.github.io/projects/DeepMimic/DeepMimic_2018.pdf)
