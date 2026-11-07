# Latent RL Prior 星系

Latent RL Priors for Data-Efficient Dexterous Manipulation

**导读** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/latent-rl-prior.md) · [原文](https://arxiv.org/abs/2611.08458v1) · [评分卡](../../leaderboard/papers/latent-rl-prior/README.md)

先微调SimToolReal teacher并收集100000条成功程序化姿态对齐轨迹，将特权历史经state tokenizer/Q-Former压为任务context；flow-matching动作transformer通过cross-attention读context，通过AdaLN读本体历史与flow time。视觉阶段冻结decoder，只以动作flow loss训练DINOv2-Small与视觉Q-Former，直接生成latent而不需要特权/latent标签；双臂的两组queries共同自注意力协调后，分别结合各臂本体进入共享单臂decoder。

## 技术挂点

- [Flow Matching](../concepts/flow.md)：给噪声到数据指定概率路径，回归沿路径的速度场；生成时数值积分这个场。

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。

- [Transformer](../concepts/transformer.md)：用注意力交换 token 信息，再逐位置加工。token 可以来自字词、图像块、状态或动作。

- [动作块](../concepts/chunk.md)：一次预测多个未来控制时刻的动作，再执行部分并用新观测更新。

- [特权训练信息](../concepts/privileged.md)：训练用额外环境真值或教师信息，部署另用可获取输入估计或模仿。

- [强化学习](../concepts/rl.md)：通过奖励和值评估改进策略，研究动作如何改变长期回报。

- [示范模仿](../concepts/imitation.md)：从专家、人类或教师策略的行为学习动作，研究数据、表示和执行误差。

- [环境适应](../concepts/adaptation.md)：根据历史观测或环境信息调整策略，使动力学或地形变化仍可处理。

- [线性探测](../concepts/linear-probe.md)：冻结编码器，用带标签的下游样本训练线性预测头，以检查特征本身是否容易迁移。

- [机器人数据与评测](../concepts/data.md)：统一观测、动作、任务与评测条件，判断数据多样性如何影响泛化。

## 本篇行星与卫星

- [Flow Matching](latent-rl-prior/flow.md) · 初读挂点
- [注意力](latent-rl-prior/attention.md) · 初读挂点
- [Transformer](latent-rl-prior/transformer.md) · 初读挂点
- [动作块](latent-rl-prior/chunk.md) · 初读挂点
- [特权训练信息](latent-rl-prior/privileged.md) · 初读挂点
- [强化学习](latent-rl-prior/rl.md) · 初读挂点
- [示范模仿](latent-rl-prior/imitation.md) · 初读挂点
- [环境适应](latent-rl-prior/adaptation.md) · 初读挂点
- [线性探测](latent-rl-prior/linear-probe.md) · 初读挂点
- [机器人数据与评测](latent-rl-prior/data.md) · 初读挂点
- [本篇方法链路](latent-rl-prior/method-chain.md) · 初读挂点
- [会控制之后，视觉该接在哪里？](latent-rl-prior/lrp-problem.md) · 初读挂点
- [两份数据不要求轨迹配对](latent-rl-prior/lrp-two-datasets.md) · 初读挂点
- [历史观测到未来动作块](latent-rl-prior/lrp-history-chunk.md) · 初读挂点
- [先收集十万条成功RL轨迹](latent-rl-prior/lrp-teacher.md) · 初读挂点
- [特权历史先变为任务context](latent-rl-prior/lrp-priv-context.md) · 初读挂点
- [动作先验学的是条件速度场](latent-rl-prior/lrp-flow.md) · 初读挂点
- [冻结decoder并保留本体条件路径](latent-rl-prior/lrp-freeze.md) · 初读挂点
- [直接预测latent，不先猜物理状态](latent-rl-prior/lrp-latent.md) · 初读挂点
- [显式桥接也只有动作监督](latent-rl-prior/lrp-explicit.md) · 初读挂点
- [两组queries协调，同一decoder分别出动作](latent-rl-prior/lrp-bimanual.md) · 初读挂点
- [三任务均为同本体仿真](latent-rl-prior/lrp-tasks.md) · 初读挂点
- [对齐成功不是十步连续达标](latent-rl-prior/lrp-criterion.md) · 初读挂点
- [少量示范仍来自另训的RL策略](latent-rl-prior/lrp-demonstrations.md) · 初读挂点
- [比较的是示范预算，不是相同训练预算](latent-rl-prior/lrp-protocol.md) · 初读挂点
- [50条抬门、1000条双臂的比较条件](latent-rl-prior/lrp-data-efficiency.md) · 初读挂点
- [精度阈值会改变优势大小](latent-rl-prior/lrp-precision.md) · 初读挂点
- [固定视觉特征后仍有先验收益](latent-rl-prior/lrp-scratch.md) · 初读挂点
- [latent接口比显式形状桥更稳](latent-rl-prior/lrp-interface-ablation.md) · 初读挂点
- [视觉小步更新，动作先验保持冻结](latent-rl-prior/lrp-adaptation-rate.md) · 初读挂点
- [训练时不见的新质量检验](latent-rl-prior/lrp-mass.md) · 初读挂点
- [能线性读出力，不等于显式力控制](latent-rl-prior/lrp-force-probe.md) · 初读挂点
- [冻结先验也会冻结能力边界](latent-rl-prior/lrp-boundaries.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
