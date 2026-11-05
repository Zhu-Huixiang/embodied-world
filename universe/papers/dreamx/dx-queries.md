# 每个潜帧只读出四个查询 · DreamX

四个可学习query汇总一个潜帧的时空表征。

1200到4是每潜帧token数压缩300倍；最长8组共32个query，每个仍有2048维，并非总计算量降低300倍。

继续拆：[直接历史读取不等于全网因果](dx-encoder-mask.md) · [编码用文字，重建用latent](dx-language.md) · [32乘2048再压成32乘32](dx-bottleneck.md) · [公共probe测表示，不是闭环成功率](dx-lary-protocol.md) · [扰动latent首先改变运动](dx-perturbation.md)。

[本篇星系](../dreamx.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamx.md) · [原文依据](https://arxiv.org/pdf/2611.05377v1)
