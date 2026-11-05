# CQL 星系

Conservative Q-Learning for Offline Reinforcement Learning

**已精讲** · 强化学习与离线决策

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md) · [原文](https://proceedings.neurips.cc/paper_files/paper/2020/hash/0d2b2061826a5df3221116a5085a6052-Abstract.html) · [评分卡](../../leaderboard/papers/cql/README.md)

CQL 在 Bellman 误差外增加正则：压低策略或广泛采样动作的 Q 值，相对抬高数据动作的 Q 值。得到的保守值函数用于策略改进，从而减少数据外动作被过高估计的风险。原文同时给出值下界分析、离散与连续控制实验及复杂数据分布比较。

## 技术挂点

- [离线强化学习](../concepts/offline.md)：从已有轨迹学习决策，训练时不能自由去环境补齐数据外动作的后果。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md#1-引言封存的数据开放的动作想象)

- [价值估计与校准](../concepts/value.md)：估计未来累积收益，再用保守、分位或参考价值等约束减少误导。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md#31-保守策略评估从逐项下压到期望下界)

- [策略与价值学习](../concepts/actor-critic.md)：actor 产生动作，critic 估计长期收益；价值估计为策略改进提供方向。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md#41-图-d-怎样接住修正后的-q)

- [softmax 与温度](../concepts/softmax.md)：对候选分数取指数后归一化为总和为 1 的概率。温度控制分差如何影响概率。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md#32-离线策略学习用-log-sum-exp-找到虚高动作)

- [强化学习](../concepts/rl.md)：通过奖励和值评估改进策略，研究动作如何改变长期回报。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md#2-预备知识高估如何钻进-bellman-目标)

- [机器人数据与评测](../concepts/data.md)：统一观测、动作、任务与评测条件，判断数据多样性如何影响泛化。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md#61-gym收益很大但不是逐行第一)

- [泛化评测与遗忘](../concepts/benchmark.md)：拆开任务、物体、场景或学习顺序，检查迁移能力和旧技能保留。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md#61-gym收益很大但不是逐行第一)

- [行为克隆](../concepts/bc.md)：直接监督观测到动作的映射，不必在每次更新中根据奖励搜索。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/cql-2006.04779/README.md#5-相关工作限制策略还是修正评分)

## 本篇行星与卫星

- [离线强化学习](cql/offline.md) · 已讲解
- [价值估计与校准](cql/value.md) · 已讲解
- [策略与价值学习](cql/actor-critic.md) · 已讲解
- [softmax 与温度](cql/softmax.md) · 已讲解
- [强化学习](cql/rl.md) · 已讲解
- [机器人数据与评测](cql/data.md) · 已讲解
- [泛化评测与遗忘](cql/benchmark.md) · 已讲解
- [行为克隆](cql/bc.md) · 已讲解
- [本篇方法链路](cql/method-chain.md) · 初读挂点
- [固定数据里的策略改进](cql/offline-fixed-data.md) · 已讲解
- [虚高估值的自举反馈](cql/bootstrap-ood-loop.md) · 已讲解
- [训练动作偏移与执行状态偏移](cql/state-action-shift.md) · 已讲解
- [奖励与旧Q组成回归目标](cql/bellman-target.md) · 已讲解
- [策略评估与策略改进交替](cql/policy-evaluation-improvement.md) · 已讲解
- [Eq1：候选动作整体受压](cql/eq1-pessimism.md) · 已讲解
- [Eq2：数据动作托住价值](cql/eq2-data-support.md) · 已讲解
- [比例修正的表格推导](cql/density-ratio-update.md) · 已讲解
- [策略期望下界](cql/expected-lower-bound.md) · 已讲解
- [CQL分布差是非负平方和](cql/cql-divergence.md) · 已讲解
- [让高Q动作成为惩罚候选](cql/adversarial-proposal.md) · 已讲解
- [CQL(H)的软最大值](cql/logsumexp.md) · 已讲解
- [一升一降来自概率之差](cql/regularizer-gradient.md) · 已讲解
- [前一策略先验的ρ变体](cql/cql-rho.md) · 已讲解
- [慢策略更新保留保守余量](cql/slow-policy.md) · 已讲解
- [扩大数据与候选的估值差](cql/gap-expansion.md) · 已讲解
- [经验MDP中的隐式策略惩罚](cql/penalized-empirical-mdp.md) · 已讲解
- [安全改进是回报比较](cql/safe-improvement.md) · 已讲解
- [有限样本改变下界余量](cql/finite-data.md) · 已讲解
- [连续动作的二路采样](cql/continuous-proposals.md) · 已讲解
- [对候选密度作重要性校正](cql/importance-correction.md) · 已讲解
- [用预算调节保守强度](cql/lagrange-budget.md) · 已讲解
- [同一正则接不同RL骨干](cql/actor-critic-qr-dqn.md) · 已讲解
- [数据动作直接提供参照](cql/no-behavior-estimator.md) · 已讲解
- [约束策略与校准Q的路线差别](cql/policy-constraint-comparison.md) · 已讲解
- [多来源Gym数据的收益与败例](cql/gym-mixtures.md) · 已讲解
- [从次优片段组合到达路径](cql/antmaze-stitching.md) · 已讲解
- [高维手部数据与行为克隆](cql/adroit-high-dimensional.md) · 已讲解
- [厨房结果锁定旧数据版](cql/kitchen-old-dataset.md) · 已讲解
- [Atari的两种数据截取](cql/atari-two-protocols.md) · 已讲解
- [用预测减真实回报检验保守性](cql/value-calibration-test.md) · 已讲解
- [随机最大Q减数据Q的诊断量](cql/gap-diagnostic.md) · 已讲解
- [删除数据支撑项的消融](cql/data-term-ablation.md) · 已讲解
- [H与ρ随动作分布改变表现](cql/variant-ablation.md) · 已讲解
- [NTK局部理论与一般深网络的距离](cql/network-theory-limit.md) · 已讲解
- [离线训练何时停仍有难题](cql/offline-early-stop.md) · 已讲解
- [仿真离线价值学习与实体部署](cql/simulation-transfer-limit.md) · 已讲解

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
