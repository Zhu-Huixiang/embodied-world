# Transformer 星系

Attention Is All You Need

**导读** · Diffusion / Transformer 基础

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/attention.md) · [原文](https://papers.nips.cc/paper/2017/hash/3f5ee243547dee91fbd053c1c4a845aa-Abstract.html) · [评分卡](../../leaderboard/papers/attention/README.md)

输入 token 先做词嵌入和位置编码，再由多头注意力计算每个位置该从哪些位置取信息。编码器使用全序列自注意力；解码器用因果遮罩阻止读取未来 token，并通过交叉注意力接收编码器输出。原文在两项 WMT 翻译任务比较质量、训练成本与不同注意力配置。

## 技术挂点

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。

- [因果序列建模](../concepts/causal.md)：通过遮罩只让位置读取允许的历史，避免训练时看到运行时不存在的未来。

- [Transformer](../concepts/transformer.md)：用注意力交换 token 信息，再逐位置加工。token 可以来自字词、图像块、状态或动作。

## 本篇行星与卫星

- [注意力](attention/attention.md) · 初读挂点
- [因果序列建模](attention/causal.md) · 初读挂点
- [Transformer](attention/transformer.md) · 初读挂点
- [本篇方法链路](attention/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
