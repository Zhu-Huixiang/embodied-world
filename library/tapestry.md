# TAPESTRY: A Single Backbone for Video Generation and Robot Control

**解读导读** · CoRL 2026 · [世界动作模型](../paper-map/README.md#track-world-action-model)

研究范围：视频预训练骨干直接输出动作块；视频任务泛化LIBERO协议及单平台双臂实机。

[原文入口](https://arxiv.org/abs/2610.36823v1) · [原文 PDF](https://arxiv.org/pdf/2610.36823v1) · [作者项目 / 代码入口](https://tapestry-wam.github.io/) · [作者与团队](../leaderboard/origins/papers/tapestry.md)

## 先看它做了什么

把每个20维动作经64×20无偏置矩阵和无仿射LayerNorm变为2×2×16伪视频patch，复用CogVideoX-2B的patch嵌入、DiT与输出层；动作读出使用同一矩阵的转置，新增1280个参数。视频、视频加动作联合、动作独立三种扩散目标共同微调骨干；联合模式动作能看视频、视频不能看动作。部署只输入干净当前观测和文字，用零末端SNR的v预测执行一步DDIM，从16个动作token得到动作块，不生成未来视频。其低噪声抖动诊断和一步采样结论依赖所用骨干、噪声日程与参数化。

## 带着什么问题读

**视频模型学会了怎样的交互规律后，机器人还必须先把未来画出来吗？能否把一个动作直接当成视频patch，只算一步就动手？**

## 为什么值得继续读

把动作接口直接对齐预训练视频patch，同时专门训练去视频的部署路径；用共享接口、训练分支、采样诊断、非标准视频迁移任务和实机消融检查效率与控制质量的取舍。

证据入口：Table 1采用LIBERO-90有动作标签、其余四suite仅提供视频的协议，每suite100次：TAPESTRY平均按表四舍五入76%，Cosmos Policy和DreamZero各70%；不是标准全监督LIBERO榜。Table 2三实机任务各10次，28/30成功，对比从零训练DiT Diffusion Policy的15/30。Table 3三项OOD各5次，10/15对DreamZero4/15，作者报告p=.07；OOD仍有对应人类视频支持。RTX5090上16动作块84ms、9GB，对优化后5B DreamZero的3.7s，速度差同时涉及模型规模、前向次数与视频token。固定5epoch消融完整模型58%，去LayerNorm33%、独立视频/动作训练36%，不能混用收敛76%。

具身关联：直接面向机器人视觉控制，研究把视频预训练中的交互知识转成低延迟动作策略；与需要在线生成未来视频的WAM形成可检验对照。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[知识星系](../universe/papers/tapestry.md) · [七维评分与雷达](../leaderboard/papers/tapestry/README.md) · [CoRL集锦](../venues/CoRL/README.md) · [地图方向](../paper-map/README.md#track-world-action-model) · [首页](../README.md)

元数据核对：2026-10-30。
