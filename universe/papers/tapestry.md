# TAPESTRY 星系

TAPESTRY: A Single Backbone for Video Generation and Robot Control

**导读** · 世界动作模型

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/tapestry.md) · [原文](https://arxiv.org/abs/2610.36823v1) · [评分卡](../../leaderboard/papers/tapestry/README.md)

把每个20维动作经64×20无偏置矩阵和无仿射LayerNorm变为2×2×16伪视频patch，复用CogVideoX-2B的patch嵌入、DiT与输出层；动作读出使用同一矩阵的转置，新增1280个参数。视频、视频加动作联合、动作独立三种扩散目标共同微调骨干；联合模式动作能看视频、视频不能看动作。部署只输入干净当前观测和文字，用零末端SNR的v预测执行一步DDIM，从16个动作token得到动作块，不生成未来视频。其低噪声抖动诊断和一步采样结论依赖所用骨干、噪声日程与参数化。

## 技术挂点

- [扩散去噪](../concepts/diffusion.md)：训练网络从带噪对象估计噪声或干净目标，生成时从噪声开始迭代恢复样本。

- [Diffusion Transformer](../concepts/dit.md)：用 Transformer 实现扩散模型的去噪网络，使 token 之间交换条件与目标信息。

- [变分自编码器 VAE](../concepts/vae.md)：编码器描述潜变量分布，解码器从潜变量重建样本，用重建与分布正则共同训练。

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。

- [动作块](../concepts/chunk.md)：一次预测多个未来控制时刻的动作，再执行部分并用新观测更新。

- [示范模仿](../concepts/imitation.md)：从专家、人类或教师策略的行为学习动作，研究数据、表示和执行误差。

- [泛化评测与遗忘](../concepts/benchmark.md)：拆开任务、物体、场景或学习顺序，检查迁移能力和旧技能保留。

- [分布偏移](../concepts/shift.md)：测试场景的画风、视角、背景或对象组合发生变化，模型习惯的视觉线索随之改变。

## 本篇行星与卫星

- [扩散去噪](tapestry/diffusion.md) · 初读挂点
- [Diffusion Transformer](tapestry/dit.md) · 初读挂点
- [变分自编码器 VAE](tapestry/vae.md) · 初读挂点
- [动作表示](tapestry/action.md) · 初读挂点
- [动作块](tapestry/chunk.md) · 初读挂点
- [示范模仿](tapestry/imitation.md) · 初读挂点
- [泛化评测与遗忘](tapestry/benchmark.md) · 初读挂点
- [分布偏移](tapestry/shift.md) · 初读挂点
- [本篇方法链路](tapestry/method-chain.md) · 初读挂点
- [把动作当成一个视频patch](tapestry/interface.md) · 初读挂点
- [复用视频输出层和转置读出](tapestry/readout.md) · 初读挂点
- [干净观测和文字前缀](tapestry/observation.md) · 初读挂点
- [三种训练目标共用一个骨干](tapestry/three-objectives.md) · 初读挂点
- [动作看视频，视频不看动作](tapestry/asymmetric-mask.md) · 初读挂点
- [把去视频部署路径也练到](tapestry/deployment-match.md) · 初读挂点
- [零末端SNR下的一步DDIM](tapestry/one-step.md) · 初读挂点
- [多步去噪为何越修越抖](tapestry/jitter.md) · 初读挂点
- [一步条件均值的多模态代价](tapestry/conditional-mean.md) · 初读挂点
- [只看目标任务视频的LIBERO协议](tapestry/libero-video.md) · 初读挂点
- [三项双臂实机与组件消融](tapestry/real-manipulation.md) · 初读挂点
- [带视频支持的OOD迁移](tapestry/ood.md) · 初读挂点
- [少token、少前向和小骨干的共同成本收益](tapestry/cost.md) · 初读挂点
- [固定5epoch的组件比较](tapestry/ablation-budget.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
