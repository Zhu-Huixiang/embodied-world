# Transformer 星系

Attention Is All You Need

**已精讲** · Diffusion / Transformer 基础

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md) · [原文](https://papers.nips.cc/paper/2017/hash/3f5ee243547dee91fbd053c1c4a845aa-Abstract.html) · [评分卡](../../leaderboard/papers/attention/README.md)

输入 token 先做词嵌入和位置编码，再由多头注意力计算每个位置该从哪些位置取信息。编码器使用全序列自注意力；解码器用因果遮罩阻止读取未来 token，并通过交叉注意力接收编码器输出。原文在两项 WMT 翻译任务比较质量、训练成本与不同注意力配置。

## 技术挂点

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md#32-注意力qkv-分工不靠玄学)

- [因果序列建模](../concepts/causal.md)：通过遮罩只让位置读取允许的历史，避免训练时看到运行时不存在的未来。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md#5-训练答案右移未来遮住)

- [Transformer](../concepts/transformer.md)：用注意力交换 token 信息，再逐位置加工。token 可以来自字词、图像块、状态或动作。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md#31-编码器与解码器两列各六层)

- [softmax 与温度](../concepts/softmax.md)：对候选分数取指数后归一化为总和为 1 的概率。温度控制分差如何影响概率。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md#32-注意力qkv-分工不靠玄学)

- [交叉熵](../concepts/cross-entropy.md)：正确候选的负对数概率。正确项概率越小，损失越大，梯度会推动正确分数上升。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/attention-1706.03762/README.md#5-训练答案右移未来遮住)

## 本篇行星与卫星

- [注意力](attention/attention.md) · 已讲解
- [因果序列建模](attention/causal.md) · 已讲解
- [Transformer](attention/transformer.md) · 已讲解
- [softmax 与温度](attention/softmax.md) · 已讲解
- [交叉熵](attention/cross-entropy.md) · 已讲解
- [本篇方法链路](attention/method-chain.md) · 初读挂点
- [跨位置的信息路径](attention/path.md) · 已讲解
- [编码器解码器堆叠](attention/stack.md) · 已讲解
- [残差后LayerNorm](attention/post-ln.md) · 已讲解
- [查询键值投影](attention/qkv.md) · 已讲解
- [缩放点积](attention/scale.md) · 已讲解
- [行softmax权重](attention/weights.md) · 已讲解
- [八头与输出投影](attention/heads.md) · 已讲解
- [三种注意力来源](attention/cross-source.md) · 已讲解
- [因果掩码](attention/causal-mask.md) · 已讲解
- [逐位置前馈层](attention/ffn.md) · 已讲解
- [词嵌入和缩放](attention/embedding.md) · 已讲解
- [正弦余弦位置编码](attention/position.md) · 已讲解
- [复杂度与顺序步数](attention/cost.md) · 已讲解
- [右移目标与teacher forcing](attention/shift.md) · 已讲解
- [标签平滑](attention/smoothing.md) · 已讲解
- [预热后衰减学习率](attention/warmup.md) · 已讲解
- [BLEU与翻译测试](attention/bleu.md) · 已讲解
- [开发集消融](attention/ablation.md) · 已讲解
- [注意力连线可视化](attention/visual.md) · 已讲解

## 论文间的联系

- [SAM](sam.md) → [Transformer](attention.md)：SAM的图像骨干与双向解码器使用Transformer注意力模块；本文在3.1–3.3拆解两路交互。 [原文定位](https://arxiv.org/abs/2304.02643v1)（§3; Appendix A）。

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
