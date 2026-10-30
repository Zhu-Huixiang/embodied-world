# SuperMimic: Scaling Humanoid Whole-Body Control with One Differentiable World Model

**SuperMimic** · CoRL 2026 · 本版排名 105 · 综合分 **78.1 / 100**

[解读导读](../../../library/supermimic.md) · [动作先验与全身技能](../../../paper-map/README.md#track-motion-priors) · [CoRL集锦](../../../venues/CoRL/README.md)

[知识星系](../../../universe/papers/supermimic.md) · [原文](https://arxiv.org/abs/2610.28480) · [PDF](https://arxiv.org/pdf/2610.28480v1) · [阅读卡片](../../../library/supermimic.md)

论文出处：[**Qiayuan Liao**](../../origins/papers/supermimic.md)<br>[伯克利混合机器人实验室](../../origins/papers/supermimic.md)

## 机制简析

先让当前策略在 MuJoCo Warp 中收集状态、动作与下一状态，存进回放池；一个共享可微动力学模型用8步自回归窗口拟合这些转移。策略更新时暂时固定模型参数，在模型里展开32步想象轨迹，把跟踪奖励经动作和状态的雅可比反传给策略，末端价值函数补上短视野外的回报。模拟器采样、世界模型拟合与策略改进交替进行，最终将跟踪策略部署到 Unitree G1。世界模型服务训练，不替换实机执行反馈。

带着这个问题读：接触动力学不光滑，为什么8步拟合的世界模型仍能给32步想象策略提供好用梯度？训练动作全覆盖又与新动作泛化差在哪里？

初读判断：共享物理动力学加短段解析梯度，直接切中大规模动作跟踪的训练成本，给创新92。主文有PPO-Sim/PPO-WM、数据规模、想象长度与critic等对照，并展示G1实机，给证据87；129,514条评测来自动作训练库、每条一次确定性播放，GPU比较硬件/数据不同，结论限定为训练动作覆盖与报告成本。附录给算法、奖励、观测和超参，官方网页有交互demo，复用70；当前项目页没有指向作者训练代码，第三方实现另列。它连接世界模型、BPTT和全身控制，阅读96。引用与传播另按当日真实快照计。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 90.0 | 30% |
| 创新性 | 92 | 20% |
| 实验与证据 | 87 | 20% |
| 学术影响 | 0.0 | 10% |
| 近期关注 | 60.4 | 5% |
| 复用价值 | 70 | 8% |
| 阅读价值 | 96 | 7% |

刊会依据：[CoRL 2026](../../../venues/CoRL/README.md)，正式出处见[出版/原文记录](https://2026.corl.org/program/accepted-papers)；采用2026-10-10刊会快照。


公开与评审依据：v1完整公开且身份、作者、时间可追溯；CoRL 2026官方录用名单含该篇，按CoRL既有90分量表取较高阶段，Oral不加分。；正式刊会按登记量表计分，取较高阶段。


编辑深度：arXiv v1主文与相关附录机制/实验初读，非完整精讲；评分记录：2026-10-27。

计量来源：OpenAlex；原研究arXiv v1索引记录；正式会议尚未出版；匹配题目：SuperMimic: Scaling Humanoid Whole-Body Control with One Differentiable World Model。累计被引 **0**，2025–2026 被引 **0**；快照：2026-10-27T14:35:45+08:00。

[指标记录](https://api.openalex.org/works/W7223142413) · [文献计量条目](https://openalex.org/W7223142413)

### 影响与关注的计算依据

- **学术影响 0.0**：身份匹配的累计引用C=0，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W7223142413)
- **近期关注 60.4**：github 的论文专属入口：第三方复现仓库star=259；按10000上限对数压缩。 [依据1](https://api.github.com/repos/CuboiLeo/SuperMimic-Reproduced) · [依据2](https://github.com/CuboiLeo/SuperMimic-Reproduced)

零分表示本次快照已定位的信号处在量表起点；创新和实验两轴分别评价方法。

### 论文公开入口与传播快照

- [project 入口](https://supermimic.github.io/)

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/CuboiLeo/SuperMimic-Reproduced) | 第三方复现仓库star 259 | 第三方单论文复现仓库，非作者官方代码；近期新建入口截至2026-10-27的累计快照 | 2026-10-27T14:35:45+08:00 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
