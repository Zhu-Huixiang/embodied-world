# ∇Mimic: Ultra-Efficient Humanoid Control with Differentiable Simulation

**解读导读** · arXiv 2026 · [动作先验与全身技能](../paper-map/README.md#track-motion-priors)

研究范围：Unitree G1平地、LAFAN1全部40动作的仿真跟踪；v1无实机与未见动作泛化评测。

[原文入口](https://arxiv.org/abs/2610.41654v1) · [原文 PDF](https://arxiv.org/pdf/2610.41654v1) · [作者项目 / 代码入口](https://sailab.ai/nablamimic/) · [作者与团队](../leaderboard/origins/papers/nablamimic.md)

本条机制与数字锁定 arXiv v1。官方项目当前另有无编号更新稿，训练配方与结果已有变化，待逐项核验后合并；不把项目稿当作 arXiv v2。

## 先看它做了什么

在4096个64步窗口中沿MuJoCo接触动力学求导，逐反向时间步对每个样本的动作cotangent按批中位范数裁剪，再以固定弧度RMS步长构造目标动作、做8次小批回归。G1专用NablaEngine用每world一个warp及整控制步adjoint megakernel降低求导成本。保留TDλ critic、参考姿态残差和回放起点；训练导数在近自接触、近平行胶囊及饱和actuator处采用特定规则，并非处处无偏的精确梯度。

## 带着什么问题读

**世界模型的收益有多少来自导数本身？把精确仿真梯度中的少数极端样本截住，再把更新改成定弧度动作目标，能否稳定而廉价地训练全身跟踪？**

## 为什么值得继续读

明确区分一阶学习失稳和仿真求导成本；裁剪/目标回归消融、同轨迹梯度尾部诊断、有限差分校验及同算法换引擎共同支持实质贡献。PODS、裁剪和回放有明确继承，不把组件集成当全部原创。

证据入口：arXiv v1 Table4：3seed/RTX PRO6000在.5/1/2/3h回报.824±.008/.854±.005/.872±.001/.875±.001，均值曲线.34h过.82。去裁剪残差3/3diverged；去多步回归残差.822对.866。Table3同GPU/4096world一步含梯度1.78ms对Warp adjoint PR20.5ms。换引擎同算法4000update .43h对2.03h；Nabla3seed、Warp1seed。SuperMimic .82/1.2h为其H100报告值，非匹配官方重跑；PPO两配置为单seed。评测全40训练库clip、确定性、跌倒余段归零、MuJoCoWarp、计时排除编译和评测。

具身关联：直接连接运动数据、全身控制、接触仿真求导与一阶强化学习，是理解SuperMimic世界模型梯度作用的具体对照。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[知识星系](../universe/papers/nablamimic.md) · [七维评分与雷达](../leaderboard/papers/nablamimic/README.md) · [arXiv集锦](../arxiv/README.md#paper-nablamimic) · [地图方向](../paper-map/README.md#track-motion-priors) · [首页](../README.md)

元数据核对：2026-11-04。
