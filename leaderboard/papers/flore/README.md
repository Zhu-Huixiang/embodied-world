# Learning Force-Reactive Humanoid Loco-Manipulation

**FLoRe** · arXiv 2026 · 本版排名 116 · 综合分 **63.0 / 100**

[解读导读](../../../library/flore.md) · [操作与动作块](../../../paper-map/README.md#track-manipulation) · [arXiv集锦](../../../arxiv/README.md#paper-flore)

[知识星系](../../../universe/papers/flore.md) · [原文](https://arxiv.org/abs/2610.35862v1) · [PDF](https://arxiv.org/pdf/2610.35862v1) · [阅读卡片](../../../library/flore.md)

论文出处：[**Sihang Li**](../../origins/papers/flore.md)<br>[亚马逊前沿人工智能与机器人团队 / 纽约大学 · 另2个机构](../../origins/papers/flore.md)

## 机制简析

双手持夹爪记录腕部图像、六轴接触力/力矩和身体运动，先做无机器人示范，再补成机器人可跟踪的全身参考。每任务一套扩散策略读取两张224×224腕图、14维相对状态和双手wrench历史，同时生成运动关键点与每手力指令；高层动作块交给低层全身控制器。低层将力误差积分换成手部位置目标偏移：命令方向持续调力，其余方向保持顺应，真实腕部传感器闭合反馈环。力不是只在训练时当标签，而是从示范、策略输入/输出一路接到执行。

带着这个问题读：位置轨迹为什么还不够？力观测、力指令与全身控制各自解决哪一步，关闭一条通道会怎样？

初读判断：创新86：核心是力标注示范、高层力输入/输出与混合顺应全身控制的贯通，建立明确的可操作接口。证据82：两条力通道的消融、同架构/数据/日程位置基线、仿真跟踪与G1实机均可定位；任务仅三类、每条件30次总rollout，去力观测的20/30到24/30不外推成显著结论。复用66：方法和控制接口清楚，采集硬件、F/T传感与每任务训练有工程成本。阅读88：适合拆解“会走会摆手”到“接触时怎样调力”的差距。影响与关注另按独立证据和计量评分。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 60 | 30% |
| 创新性 | 86 | 20% |
| 实验与证据 | 82 | 20% |
| 学术影响 | 0 | 10% |
| 近期关注 | 0 | 5% |
| 复用价值 | 66 | 8% |
| 阅读价值 | 88 | 7% |

公开与评审依据：arXiv v1完整公开，稳定论文身份、作者和时间可追溯，按完整公开阶段60计；当前阶段为预印本公开。


编辑深度：arXiv v1方法/全部实验与相关附录初读，非完整精讲；评分记录：2026-10-28。

累计引用与近期引用尚未匹配；原始值保留null。下面列出已定位的评分信号。

### 影响与关注的计算依据

- **学术影响 0**：本次有界补查未核到独立研究采用，按独立采用量表起点0计；引用接口受限/尚未匹配，原始引用为null，这个分数不等于被引0。 [依据1](https://arxiv.org/abs/2610.35862v1) · [依据2](https://api.github.com/search/repositories?q=2610.35862&per_page=10) · [依据3](https://huggingface.co/api/papers/2610.35862)
- **近期关注 0**：本次未取得可核的单篇平台计数或近期独立技术采用，按证据量表起点0计；自动摘要转载与共享索引不赋关注分，不能据此说论文无人关注。 [依据1](https://arxiv.org/abs/2610.35862v1) · [依据2](https://api.github.com/search/repositories?q=2610.35862&per_page=10) · [依据3](https://huggingface.co/api/papers/2610.35862)

零分表示本次快照已定位的信号处在量表起点；创新和实验两轴分别评价方法。

### 论文公开入口与传播快照

- [project 入口](https://louis-leee.github.io/FLoRe/)

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
