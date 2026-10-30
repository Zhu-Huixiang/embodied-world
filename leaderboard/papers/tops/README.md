# TOPS: Reshaping Flow Source and Transport for Multi-Task Robot Manipulation

**TOPS** · arXiv 2026 · 本版排名 112 · 综合分 **65.0 / 100**

[解读导读](../../../library/tops.md) · [操作与动作块](../../../paper-map/README.md#track-manipulation) · [arXiv集锦](../../../arxiv/README.md#paper-tops)

[知识星系](../../../universe/papers/tops.md) · [原文](https://arxiv.org/abs/2610.36694v1) · [PDF](https://arxiv.org/pdf/2610.36694v1) · [阅读卡片](../../../library/tops.md)

论文出处：[**Tuo An**](../../origins/papers/tops.md)<br>[南洋理工大学 MARS 实验室](../../origins/papers/tops.md)

## 机制简析

先用标准flow matching暖启动，把专家动作块沿逆流拉回噪声空间，按训练任务建立bank，再以低秩协方差高斯混合MPPCA拟合任务源。根据源/动作协方差的高斯最优输运方向识别需要扩张的轴，只在这些方向采用先慢后快插值，其他方向保留线性。固定源和schedule继续训练同一速度网络；语言selector选已知任务源。推理的一步采用依序两次网络求值的schedule-aware两半步方法，即NFE=2，不是一次前向。

带着这个问题读：多任务动作流为什么都要从同一个高斯出发、沿同一条直线走？换出发点和速度安排，能否少算几次网络？

初读判断：创新88：将逆流任务源、协方差方向时序和专用两阶段求解器连接起来，网络结构不变；高斯端点理论只支持限定模型下的风险上界分析。证据87：主表三训练run、source/path消融、匹配NFE诊断、π0.5迁移和八类实机任务覆盖较完整；已知任务集合、π0.5单checkpoint与固定身体单臂范围需保留，主表与诊断的混合成分数不同。复用70：算法、超参、实现细节和推导可追溯，项目Code按钮仍为占位，离线source/schedule准备有成本。阅读92：适合解释动作生成中起点、路径和求解器三者如何共同影响少步采样。影响与近期关注依外部证据另计。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 60 | 30% |
| 创新性 | 88 | 20% |
| 实验与证据 | 87 | 20% |
| 学术影响 | 0 | 10% |
| 近期关注 | 0 | 5% |
| 复用价值 | 70 | 8% |
| 阅读价值 | 92 | 7% |

公开与评审依据：arXiv v1完整公开，稳定身份、版本与作者可追溯，按公开阶段60计。；当前阶段为预印本公开。


编辑深度：arXiv v1主文方法/实验及相关附录初读；A9长证明未逐行验算，非完整精讲；评分记录：2026-10-29。

累计引用与近期引用尚未匹配；原始值保留null。下面列出已定位的评分信号。

### 影响与关注的计算依据

- **学术影响 0**：本次有界补查未核到独立技术采用，按证据量表起点0；原始引用未匹配为null，非实测零引用。 [依据1](https://arxiv.org/abs/2610.36694v1) · [依据2](https://ntumars.github.io/TOPS/) · [依据3](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2610.36694?fields=title,authors,year,externalIds,citationCount,citations.paperId,citations.year) · [依据4](https://api.openalex.org/works/https://doi.org/10.48550/arxiv.2610.36694) · [依据5](https://api.openalex.org/works?search=TOPS%3A+Reshaping+Flow+Source+and+Transport+for+Multi-Task+Robot+Manipulation&per-page=5) · [依据6](https://huggingface.co/api/papers/2610.36694) · [依据7](https://api.github.com/search/repositories?q=2610.36694&per_page=10)
- **近期关注 0**：本次未取得可核单篇计数或近期独立采用，按证据量表起点0；实际取得的平台量仍按量表另取较高值。 [依据1](https://arxiv.org/abs/2610.36694v1) · [依据2](https://ntumars.github.io/TOPS/) · [依据3](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2610.36694?fields=title,authors,year,externalIds,citationCount,citations.paperId,citations.year) · [依据4](https://api.openalex.org/works/https://doi.org/10.48550/arxiv.2610.36694) · [依据5](https://api.openalex.org/works?search=TOPS%3A+Reshaping+Flow+Source+and+Transport+for+Multi-Task+Robot+Manipulation&per-page=5) · [依据6](https://huggingface.co/api/papers/2610.36694) · [依据7](https://api.github.com/search/repositories?q=2610.36694&per_page=10)

零分表示本次快照已定位的信号处在量表起点；创新和实验两轴分别评价方法。

### 论文公开入口与传播快照

- [project 入口](https://ntumars.github.io/TOPS/)

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
