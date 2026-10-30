# Gaussian Distillation of Flow Policies

**GAR** · arXiv 2026 · 本版排名 122 · 综合分 **61.0 / 100**

[解读导读](../../../library/gar.md) · [操作与动作块](../../../paper-map/README.md#track-manipulation) · [arXiv集锦](../../../arxiv/README.md#paper-gar)

[知识星系](../../../universe/papers/gar.md) · [原文](https://arxiv.org/abs/2610.40271v1) · [PDF](https://arxiv.org/pdf/2610.40271v1) · [阅读卡片](../../../library/gar.md)

论文出处：[**Youssef Saied**](../../origins/papers/gar.md)<br>[日内瓦大学 / 图宾根大学 · 另2个机构](../../origins/papers/gar.md)

## 机制简析

GAR冻结原策略的视觉语言骨干和动作Transformer，把固定噪声在t=0的一次前向特征接给小读出：仿射修正预测连续动作均值，池化后128单元MLP预测方差或Cholesky因子，另一仿射头预测离散命令的伯努利概率。训练目标来自已部署教师反复采样的经验矩与命令频率，均值用最小二乘，协方差用按坐标归一的误差及对数方差项，离散命令用交叉熵。推理直接采样高斯连续动作和独立伯努利命令，不再积分速度场；可写闭式动作似然。论文先检验固定观测下教师平移/旋转分布的高斯近似，再检查控制表现和近似的代价。

带着这个问题读：动作流真的需要反复积分才能做得好，还是冻结内部特征后，用一个高斯读出就能保留大部分控制能力？

初读判断：创新75：用冻结flow内部特征学习连续高斯矩与离散命令概率，改变多步采样接口，且把单峰条件动作与多路径闭环行为分开；单步均值恒等式及蒸馏已有先例。证据82：两RoboCasa教师、50任务各50次、LIBERO补测、均值/协方差/固定噪声与成本消融较完整；主要任务表为单拟合checkpoint、全部仿真，不能把区间含零写成等效。复用72：读出模块小，训练目标、正则、缓存和推理路径细节可追溯；教师统计准备昂贵，当前未核到公开实现。阅读84：连接flow速度场、高斯矩、动作似然与闭环多样性的实用桥梁，不把近高斯观察推广到所有机器人策略。影响/关注按已核单篇信号另计，不借教师或作者声望。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 60 | 30% |
| 创新性 | 75 | 20% |
| 实验与证据 | 82 | 20% |
| 学术影响 | 0 | 10% |
| 近期关注 | 0 | 5% |
| 复用价值 | 72 | 8% |
| 阅读价值 | 84 | 7% |

公开与评审依据：完整公开稿阶段60。；当前阶段为预印本公开。


编辑深度：完整读取v1共35页主文与附录，核对主要公式定义、协议、表格、CI与成本；未执行代码复现、未逐行独立重证全部理论推导，不等于完整公开精讲。；评分记录：2026-10-30。

累计引用与近期引用尚未匹配；原始值保留null。下面列出已定位的评分信号。

### 影响与关注的计算依据

- **学术影响 0**：S2精确arXiv ID限流，OpenAlex精确DOI未匹配，标题检索前5为其他论文；未核到独立技术采用。采用量表起点0，原始引用为null，不是实测零引用。 [依据1](https://arxiv.org/abs/2610.40271v1) · [依据2](https://arxiv.org/pdf/2610.40271v1) · [依据3](https://youssefsaied.github.io/) · [依据4](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2610.40271?fields=title,authors,year,citationCount,influentialCitationCount,externalIds,url,publicationVenue,publicationTypes) · [依据5](https://api.openalex.org/works/https://doi.org/10.48550/arXiv.2610.40271) · [依据6](https://api.openalex.org/works?search=Gaussian%20Distillation%20of%20Flow%20Policies&per-page=5) · [依据7](https://huggingface.co/api/papers/2610.40271)
- **近期关注 0**：HF单篇404，GitHub精确ID/完整标题前10为空，第一作者官网暂无本篇入口，未取得单篇计数或独立采用。当前证据量表起点0，未知原始关注数为null。 [依据1](https://arxiv.org/abs/2610.40271v1) · [依据2](https://arxiv.org/pdf/2610.40271v1) · [依据3](https://youssefsaied.github.io/) · [依据4](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2610.40271?fields=title,authors,year,citationCount,influentialCitationCount,externalIds,url,publicationVenue,publicationTypes) · [依据5](https://api.openalex.org/works/https://doi.org/10.48550/arXiv.2610.40271) · [依据6](https://api.openalex.org/works?search=Gaussian%20Distillation%20of%20Flow%20Policies&per-page=5) · [依据7](https://huggingface.co/api/papers/2610.40271)

零分表示本次快照已定位的信号处在量表起点；创新和实验两轴分别评价方法。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
