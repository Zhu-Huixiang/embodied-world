# 模型预测控制 MPC

在模型里比较未来动作序列，执行开头一段，用新观测重算下一轮。

CEM 等搜索器负责提出和筛选序列，模型负责预测。

分类上层：[世界模型](world.md)。

## 哪些论文用到或讨论它

- [TD-MPC](../papers/td-mpc.md) · 机制导读 · [原文](https://proceedings.mlr.press/v162/hansen22a.html)
- [TD-MPC2](../papers/td-mpc2.md) · 机制导读 · [原文](https://proceedings.iclr.cc/paper_files/paper/2024/hash/cf73d57b6dcda32b293df7c2d5341f49-Abstract-Conference.html)
- [LeWM](../papers/lewm.md) · 机制导读 · [原文](https://arxiv.org/abs/2603.19312v1)
- [V-JEPA 2](../papers/vjepa2.md) · 机制导读 · [原文](https://arxiv.org/abs/2506.09985)
- [LeWAM](../papers/lewam.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.12407v1)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
