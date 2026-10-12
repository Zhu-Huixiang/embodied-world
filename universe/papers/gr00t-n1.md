# GR00T N1 星系

GR00T N1: An Open Foundation Model for Generalist Humanoid Robots

**导读** · 视觉语言动作模型 VLA

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/gr00t-n1.md) · [原文](https://arxiv.org/abs/2503.14734) · [评分卡](../../leaderboard/papers/gr00t-n1/README.md)

Eagle-2视觉语言middle-layer tokens→DiT交叉注意力；embodiment-specific MLP编码state与noisy action、解码H=16连续动作块，flow-matching训练、K=4步采样。人类latent-action、real robot、DexMimicGen模拟和生成视频IDM/LAPA伪动作组成数据金字塔。

## 技术挂点

- [Flow Matching](../concepts/flow.md)：给噪声到数据指定概率路径，回归沿路径的速度场；生成时数值积分这个场。

- [Diffusion Transformer](../concepts/dit.md)：用 Transformer 实现扩散模型的去噪网络，使 token 之间交换条件与目标信息。

- [跨本体数据](../concepts/cross-body.md)：从多个机器人或人类收集经验，通过动作/观测适配接到共享学习系统。

## 本篇行星与卫星

- [Flow Matching](gr00t-n1/flow.md) · 初读挂点
- [Diffusion Transformer](gr00t-n1/dit.md) · 初读挂点
- [跨本体数据](gr00t-n1/cross-body.md) · 初读挂点
- [本篇方法链路](gr00t-n1/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
