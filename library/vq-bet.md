# Behavior Generation with Latent Actions

出处：ICML 2024。研究范围：VQ-BeT、残差向量量化与多模态行为生成。

[原文入口](https://proceedings.mlr.press/v235/lee24y.html) · [原文 PDF](https://raw.githubusercontent.com/mlresearch/v235/main/assets/lee24y/lee24y.pdf) · [作者项目 / 代码入口](https://sjlee.cc/vq-bet/)

ICML 2024 正式版，作者项目记 Spotlight；不是 RSS。原文不同设置的速度比不同，不能把某一速度倍率套全篇。

阅读问题：**动作先压成分层离散码，能否保留多种操作方式，同时省掉扩散反复采样？**

收录理由：动作 token 路线与扩散策略的清楚对照，连接 BeT、分层量化以及后续高效动作生成。

证据入口：ICML 正式稿与项目提供与 BeT、Diffusion Policy 的多任务和速度对照，真实长程任务与开放实现支撑复用；部分任务没有优势，评分以整体机制和证据覆盖为准。

具身关联：动作 token 路线与扩散策略的清楚对照，连接 BeT、分层量化以及后续高效动作生成。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/vq-bet/README.md)

机制简析：第一阶段用残差向量量化编码器把连续动作或动作块压成分层码，解码器还原动作；第二阶段 Transformer 根据观测与可选目标预测这些离散码和修正量。一次前向生成替代扩散多步去噪，同时保留行为分布的多种模式。原文比较条件/无条件任务、仿真和真实长程操作，以及推理时延。
<!-- discovery:end -->
