# 对候选密度作重要性校正 · CQL

用各自采样密度修正指数Q，近似连续动作积分。

批次候选可组织成B×20×d_a，经critic得到B×20个分数，再沿动作轴归约；采样仍是有限近似。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md#42-连续动作无穷多个怎么求和)

[本篇星系](../cql.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md) · [原文依据](https://papers.nips.cc/paper_files/paper/2020/file/0d2b2061826a5df3221116a5085a6052-Supplemental.pdf)
