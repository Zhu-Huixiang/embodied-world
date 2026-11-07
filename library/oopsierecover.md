# OopsieRecover: Learning Transferable VLA Corrections from Semantic Interventions

**解读导读** · arXiv 2026 · [操作与动作块](../paper-map/README.md#track-manipulation)

研究范围：冻结π0.5的局部语义纠正；RoboCasa三仿真任务和DROID三实机任务的位姿/场景变化。实机指标为完成阶段比例，非完整任务成功率。

[原文入口](https://arxiv.org/abs/2611.08462v1) · [原文 PDF](https://arxiv.org/pdf/2611.08462v1) · [作者项目 / 代码入口](https://robin-lab.cs.utexas.edu/oopsierecover/) · [作者与团队](../leaderboard/origins/papers/oopsierecover.md)

所读9页arXiv v1与官方8页PDF有差异。实机结果按完成阶段比例报告；正文与图线不一致的Fig5精确峰值留待更正。

## 先看它做了什么

人接管时提供纠正轨迹、语言和纠正类别。VLM选语义实体种子，分割与深度把区域变成3D点集，质心时间轨迹用于生成gate×(纠正代价+λ任务代价)。触发阈值从同类记录中gate=1的干预前分数取最小；用人类/后续基策略窗口的较低成本及触发检查做经验一致性核验，失败促使程序细化，但预算耗尽仍保留最后程序。部署重新定位实体，从冻结π0.5采样动作块并可加cardinal actions，预测点集后按折扣成本筛最优；仿真用模拟器物理，实机用grasp-based近似。

## 带着什么问题读

**纠正机器人一次，它记住的是那条手的轨迹，还是“别碰到咖啡机”这条规则？把几何意图单独存起来，能否在换场景后继续帮冻结VLA选动作？**

## 为什么值得继续读

完整v1机制、同干预数据对照、三任务仿真迁移与实机progress支持有限系统贡献。按预印本原文导读收录；保留无组件消融、阶段评分细则和运行配置缺失，不用有争议峰值抬高结论。

证据入口：Fig4三仿真任务每任务5–8次纠正，对照同数据HG-DAgger*/OLAF及仅任务文字VLS；按三任务汇总且论文称每方法50episodes，L1/L2为独立最佳统计组、L0与HG共享组。DROID三任务每任务3–6纠正，官网明确20rollouts/方法/任务/level；作者报告task progress均值从基策略π0.5的35.1%升至61.0%，L0/L2与基策略分开而L1不分开，未给逐任务stage表。Q3单次纠正在10个陌生场景均触发并避免蒸汽手柄碰撞100步。无组件消融，Fig5峰值/比较次数文本存在冲突，不采用其精确峰值；也不把局部避碰称通用安全。

具身关联：直接处理机器人部署中的人类纠正、语义几何接地、动作候选预测与实机反馈，连接模仿学习和测试时策略修正。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[知识星系](../universe/papers/oopsierecover.md) · [七维评分与雷达](../leaderboard/papers/oopsierecover/README.md) · [arXiv集锦](../arxiv/README.md#paper-oopsierecover) · [地图方向](../paper-map/README.md#track-manipulation) · [首页](../README.md)

元数据核对：2026-11-07。
