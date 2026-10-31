# world2vec: Mechanistic world models through latent dynamics learning

**world2vec** · arXiv 2026 · 本版排名 123 · 综合分 **57.9 / 100**

[解读导读](../../../library/world2vec.md) · [世界模型与模型强化学习](../../../paper-map/README.md#track-world-model) · [arXiv集锦](../../../arxiv/README.md#paper-world2vec)

[知识星系](../../../universe/papers/world2vec.md) · [原文](https://arxiv.org/abs/2610.40637v1) · [PDF](https://arxiv.org/pdf/2610.40637v1) · [阅读卡片](../../../library/world2vec.md)

论文出处：[**Tobias Schmidt / Rodrigo Gonzalez Laiz**](../../origins/papers/world2vec.md)<br>[亥姆霍兹慕尼黑中心 / 慕尼黑机器学习中心 · 另1个机构](../../origins/papers/world2vec.md)

## 机制简析

world2vec用三帧观测编码潜状态，MLP预测动作条件变化率，以Euler残差积分出多步潜轨迹；把每一步预测对齐真实未来编码，以SIGReg或DCL防止表示塌缩。超参选择用未来检索EQA，另报告跨seed仿射一致性和LRC。执行时编码目标观测，CEM按潜距离选动作并滚动重规划，不训练奖励模型。科学辨识实验另将向量场换成稀疏多项式库，在已知最高阶和仿射坐标不确定性下读出动力学关系。

带着这个问题读：世界模型拿高回报，就等于真的学会物理规律了吗？把下一状态预测换成潜速度场，再沿自己的预测轨迹训练，能让控制与动力学忠实度一起提高吗？

初读判断：创新74：潜变化率、多步自身rollout匹配、防塌缩先验与忠实度指标形成可控/可解释模型接口；ODE积分、残差、多步损失和SINDy各有先例。证据72：两项核心消融、LeWM原协议、混合难度和71系统补充；三项简化仿真、视觉CartPole失败、跨法数据/奖励/频率差异及符号验证集报告使证据未达80档。复用62：公式、训练和规划参数可学习，小模型便于机制研究；官方代码未发布，不因仓库入口加分。阅读82：拆开模型自洽、可辨识性与控制成功，直接连接现有LeWM/TD-MPC2/Dreamer问题。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 60 | 30% |
| 创新性 | 74 | 20% |
| 实验与证据 | 72 | 20% |
| 学术影响 | 0 | 10% |
| 近期关注 | 0 | 5% |
| 复用价值 | 62 | 8% |
| 阅读价值 | 82 | 7% |

公开与评审依据：完整可追溯公开稿60；未核正式录用或独立技术检验，不借机构/聚合页加分。；当前阶段为预印本公开。


编辑深度：完整阅读19页v1正文/参考文献/附录A–F，目视PDF1/5/6/7/8/9/16/18/19完整页；核控制协议、消融、符号报告集与择优展示。未执行代码复现，不等于公开完整精讲。；评分记录：2026-10-31。

累计引用与近期引用尚未匹配；原始值保留null。下面列出已定位的评分信号。

### 影响与关注的计算依据

- **学术影响 0**：引用源未匹配；全文、官方项目及精确ID搜索前5未定位独立技术采用，量表起点0。原始引用null，作者其他工作与摘要聚合不算本篇采用。 [依据1](https://arxiv.org/abs/2610.40637v1) · [依据2](https://arxiv.org/pdf/2610.40637v1) · [依据3](https://worldmodels.science/world2vec/) · [依据4](https://github.com/dynamical-inference/world2vec) · [依据5](https://raw.githubusercontent.com/dynamical-inference/world2vec/main/README.md) · [依据6](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2610.40637?fields=title,authors,year,publicationDate,venue,citationCount,influentialCitationCount,externalIds,url) · [依据7](https://api.openalex.org/works/https://doi.org/10.48550/arXiv.2610.40637) · [依据8](https://api.openalex.org/works?search=world2vec%3A%20Mechanistic%20world%20models%20through%20latent%20dynamics%20learning&per-page=5) · [依据9](https://huggingface.co/api/papers/2610.40637)
- **近期关注 0**：单篇GitHub实测star/fork/subscriber均0，HF单篇upvote实测0；未核带计数独立讨论，当前关注分0。引用/网页阅读量/X保持null，不借实验室账号流量。 [依据1](https://arxiv.org/abs/2610.40637v1) · [依据2](https://arxiv.org/pdf/2610.40637v1) · [依据3](https://worldmodels.science/world2vec/) · [依据4](https://github.com/dynamical-inference/world2vec) · [依据5](https://raw.githubusercontent.com/dynamical-inference/world2vec/main/README.md) · [依据6](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2610.40637?fields=title,authors,year,publicationDate,venue,citationCount,influentialCitationCount,externalIds,url) · [依据7](https://api.openalex.org/works/https://doi.org/10.48550/arXiv.2610.40637) · [依据8](https://api.openalex.org/works?search=world2vec%3A%20Mechanistic%20world%20models%20through%20latent%20dynamics%20learning&per-page=5) · [依据9](https://huggingface.co/api/papers/2610.40637)

零分表示本次快照已定位的信号处在量表起点；创新和实验两轴分别评价方法。

### 论文公开入口与传播快照

- [project 入口](https://worldmodels.science/world2vec/)

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/dynamical-inference/world2vec) | GitHub Star 0；GitHub Watch订阅 0；GitHub Fork 0 | 单篇论文官方仓库入口；截至2026-10-31的累计快照 | 2026-10-31T08:42:23.780517+08:00 |
| [huggingface](https://huggingface.co/papers/2610.40637) | HF论文upvote 0 | single_paper；截至2026-10-31单篇计数 | 2026-10-31T08:42:23.780517+08:00 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
