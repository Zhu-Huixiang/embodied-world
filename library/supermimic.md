# SuperMimic: Scaling Humanoid Whole-Body Control with One Differentiable World Model

**解读导读** · CoRL 2026 · [动作先验与全身技能](../paper-map/README.md#track-motion-priors)

研究范围：模型强化学习驱动的人形全身动作跟踪；平地动作库与G1实机迁移。

[原文入口](https://arxiv.org/abs/2610.28480) · [原文 PDF](https://arxiv.org/pdf/2610.28480v1) · [作者项目 / 代码入口](https://supermimic.github.io/) · [作者与团队](../leaderboard/origins/papers/supermimic.md)

CoRL 2026已录用，官方名单Oral O7、poster 217；展示形式不额外加分。

## 先看它做了什么

先让当前策略在 MuJoCo Warp 中收集状态、动作与下一状态，存进回放池；一个共享可微动力学模型用8步自回归窗口拟合这些转移。策略更新时暂时固定模型参数，在模型里展开32步想象轨迹，把跟踪奖励经动作和状态的雅可比反传给策略，末端价值函数补上短视野外的回报。模拟器采样、世界模型拟合与策略改进交替进行，最终将跟踪策略部署到 Unitree G1。世界模型服务训练，不替换实机执行反馈。

## 带着什么问题读

**接触动力学不光滑，为什么8步拟合的世界模型仍能给32步想象策略提供好用梯度？训练动作全覆盖又与新动作泛化差在哪里？**

## 为什么值得继续读

用共享可微动力学把全身动作跟踪的训练成本降下来；策略梯度来源、模型/策略交替、数据扩展与覆盖评测都有可定位实验，适合作为世界模型接入底层控制的重点案例。

证据入口：§4.1/Fig.3：1 H100训练3h回报超过已发布SONIC；Appendix F/Table A.8：同一129,514训练动作库SONIC失败179、SuperMimic 1GPU/3h失败25、2GPU/9.8h失败0。硬件与训练数据不同；这组是训练库覆盖，不是未见动作测试。

具身关联：共享动力学、短段想象和价值引导直接用于G1动作跟踪及实机迁移。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[知识星系](../universe/papers/supermimic.md) · [七维评分与雷达](../leaderboard/papers/supermimic/README.md) · [CoRL集锦](../venues/CoRL/README.md) · [地图方向](../paper-map/README.md#track-motion-priors) · [首页](../README.md)

元数据核对：2026-10-27。
