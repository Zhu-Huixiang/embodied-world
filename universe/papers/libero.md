# LIBERO 星系

LIBERO: Benchmarking Knowledge Transfer for Lifelong Robot Learning

**导读** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/libero.md) · [原文](https://proceedings.neurips.cc/paper_files/paper/2023/hash/8c3c666820ea055a77726d66fc7d447f-Abstract.html) · [评分卡](../../leaderboard/papers/libero/README.md)

程序化构造物体、空间、目标和长任务不同组合，把迁移对象拆成概念知识与执行知识；模型按任务顺序学习，在新任务上只能有限访问旧数据。评测分别检查前向迁移、遗忘、任务顺序和预训练作用。原文比较顺序微调、回放和保留参数等办法，发现某些防遗忘方法会压制新任务学习。

## 技术挂点

- [泛化评测与遗忘](../concepts/benchmark.md)：拆开任务、物体、场景或学习顺序，检查迁移能力和旧技能保留。

- [行为克隆](../concepts/bc.md)：直接监督观测到动作的映射，不必在每次更新中根据奖励搜索。

- [机器人数据与评测](../concepts/data.md)：统一观测、动作、任务与评测条件，判断数据多样性如何影响泛化。

## 本篇行星与卫星

- [泛化评测与遗忘](libero/benchmark.md) · 初读挂点
- [行为克隆](libero/bc.md) · 初读挂点
- [机器人数据与评测](libero/data.md) · 初读挂点
- [本篇方法链路](libero/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
