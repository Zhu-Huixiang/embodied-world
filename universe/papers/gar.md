# GAR 星系

Gaussian Distillation of Flow Policies

**导读** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/gar.md) · [原文](https://arxiv.org/abs/2610.40271v1) · [评分卡](../../leaderboard/papers/gar/README.md)

GAR冻结原策略的视觉语言骨干和动作Transformer，把固定噪声在t=0的一次前向特征接给小读出：仿射修正预测连续动作均值，池化后128单元MLP预测方差或Cholesky因子，另一仿射头预测离散命令的伯努利概率。训练目标来自已部署教师反复采样的经验矩与命令频率，均值用最小二乘，协方差用按坐标归一的误差及对数方差项，离散命令用交叉熵。推理直接采样高斯连续动作和独立伯努利命令，不再积分速度场；可写闭式动作似然。论文先检验固定观测下教师平移/旋转分布的高斯近似，再检查控制表现和近似的代价。

## 技术挂点

- [教师学生蒸馏](../concepts/distill.md)：用教师的预测或动作监督学生，让部署模型复制可用行为。

- [Flow Matching](../concepts/flow.md)：给噪声到数据指定概率路径，回归沿路径的速度场；生成时数值积分这个场。

- [条件生成](../concepts/generation.md)：从一个条件生成多个可能输出，学习图像、视频或动作的分布而非只给一个均值。

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。

- [动作块](../concepts/chunk.md)：一次预测多个未来控制时刻的动作，再执行部分并用新观测更新。

- [Transformer](../concepts/transformer.md)：用注意力交换 token 信息，再逐位置加工。token 可以来自字词、图像块、状态或动作。

- [示范模仿](../concepts/imitation.md)：从专家、人类或教师策略的行为学习动作，研究数据、表示和执行误差。

- [泛化评测与遗忘](../concepts/benchmark.md)：拆开任务、物体、场景或学习顺序，检查迁移能力和旧技能保留。

- [闭环滚动与历史偏移](../concepts/rollout.md)：重复预测、执行或生成，把新观测或模型历史接回后续计算。

## 本篇行星与卫星

- [教师学生蒸馏](gar/distill.md) · 初读挂点
- [Flow Matching](gar/flow.md) · 初读挂点
- [条件生成](gar/generation.md) · 初读挂点
- [动作表示](gar/action.md) · 初读挂点
- [动作块](gar/chunk.md) · 初读挂点
- [Transformer](gar/transformer.md) · 初读挂点
- [示范模仿](gar/imitation.md) · 初读挂点
- [泛化评测与遗忘](gar/benchmark.md) · 初读挂点
- [闭环滚动与历史偏移](gar/rollout.md) · 初读挂点
- [本篇方法链路](gar/method-chain.md) · 初读挂点
- [动作分布的复杂度与控制代价](gar/objective.md) · 初读挂点
- [固定观测下的高斯近似](gar/gaussian-test.md) · 初读挂点
- [零时刻速度场与条件均值](gar/mean-identity.md) · 初读挂点
- [方差与内部特征](gar/variance.md) · 初读挂点
- [冻结骨干的一次前向](gar/frozen-path.md) · 初读挂点
- [均值与协方差读出](gar/heads.md) · 初读挂点
- [离散命令的probit读出](gar/binary.md) · 初读挂点
- [教师采样目标与数据划分](gar/teacher-targets.md) · 初读挂点
- [三种读出目标与训练](gar/losses.md) · 初读挂点
- [0.02%状态背后的准备成本](gar/preparation.md) · 初读挂点
- [一步采样与闭式似然](gar/sampling.md) · 初读挂点
- [两教师与两仿真基准](gar/control.md) · 初读挂点
- [动作网络次数与全策略延迟](gar/latency.md) · 初读挂点
- [成功率差的不确定度](gar/uncertainty.md) · 初读挂点
- [分布形状与矩预测误差](gar/shape-moment.md) · 初读挂点
- [单峰动作与多路径闭环行为](gar/feedback-diversity.md) · 初读挂点
- [近似模型与迁移边界](gar/limits.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
