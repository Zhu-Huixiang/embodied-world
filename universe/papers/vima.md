# VIMA 星系

VIMA: Robot Manipulation with Multimodal Prompts

**导读** · 视觉语言动作模型 VLA

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/vima.md) · [原文](https://proceedings.mlr.press/v202/jiang23b.html) · [评分卡](../../leaderboard/papers/vima/README.md)

对象图像 token 与文字交错构成任务提示，再经 T5 编码；因果 Transformer 通过交叉注意力读取提示，并结合交互历史自回归输出动作。程序化生成任务按不同泛化难度拆开测试，避免只看训练分布平均成功率。原文对对象 tokenizer、提示接入方式、模型规模和数据量分别消融。

## 技术挂点

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。

- [因果序列建模](../concepts/causal.md)：通过遮罩只让位置读取允许的历史，避免训练时看到运行时不存在的未来。

- [泛化评测与遗忘](../concepts/benchmark.md)：拆开任务、物体、场景或学习顺序，检查迁移能力和旧技能保留。

## 本篇行星与卫星

- [注意力](vima/attention.md) · 初读挂点
- [因果序列建模](vima/causal.md) · 初读挂点
- [泛化评测与遗忘](vima/benchmark.md) · 初读挂点
- [本篇方法链路](vima/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
