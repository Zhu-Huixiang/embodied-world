# 残差向量量化 RVQ

用第一层码近似向量，再用后续码近似剩余误差，最后把各层码相加重建。

Holo-M 使用四级码；层级是逐次补误差，不是四个独立动作。

分类上层：[离散编码与量化](quantization.md)。

## 在完整解读里看计算与例子

- [Holo-M：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/holo-m-2609.35709/README.md#31-统一动作编码208究竟怎么算出来的)

## 哪些论文用到或讨论它

- [Holo-M](../papers/holo-m.md) · 已精讲 · [原文](https://arxiv.org/abs/2609.35709v1)
- [VQ-BeT](../papers/vq-bet.md) · 机制导读 · [原文](https://proceedings.mlr.press/v235/lee24y.html)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
