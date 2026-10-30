# TAPESTRY: A Single Backbone for Video Generation and Robot Control

**TAPESTRY** · CoRL 2026 · 本版排名 109 · 综合分 **69.6 / 100**

[解读导读](../../../library/tapestry.md) · [世界动作模型](../../../paper-map/README.md#track-world-action-model) · [CoRL集锦](../../../venues/CoRL/README.md)

[知识星系](../../../universe/papers/tapestry.md) · [原文](https://arxiv.org/abs/2610.36823v1) · [PDF](https://arxiv.org/pdf/2610.36823v1) · [阅读卡片](../../../library/tapestry.md)

论文出处：[**Jeremy A. Collins**](../../origins/papers/tapestry.md)<br>[佐治亚理工学院 / 马里兰大学 · 另1个机构](../../origins/papers/tapestry.md)

## 机制简析

把每个20维动作经64×20无偏置矩阵和无仿射LayerNorm变为2×2×16伪视频patch，复用CogVideoX-2B的patch嵌入、DiT与输出层；动作读出使用同一矩阵的转置，新增1280个参数。视频、视频加动作联合、动作独立三种扩散目标共同微调骨干；联合模式动作能看视频、视频不能看动作。部署只输入干净当前观测和文字，用零末端SNR的v预测执行一步DDIM，从16个动作token得到动作块，不生成未来视频。其低噪声抖动诊断和一步采样结论依赖所用骨干、噪声日程与参数化。

带着这个问题读：视频模型学会了怎样的交互规律后，机器人还必须先把未来画出来吗？能否把一个动作直接当成视频patch，只算一步就动手？

初读判断：创新78：以单动作单patch、共享预训练输入/输出和三目标连接视频生成与动作控制，改变重要接口；共享骨干、视频监督与一步策略有既有路线。证据78：非标准LIBERO四suite各100次、实机同分布30次/OOD15次、固定预算组件消融与采样诊断相互支撑；实机范围和样本量有限，OOD对DreamZero差异p=.07，像素频谱不能直接证明latent空间因果机制。复用65：超参与数据路由清楚，行动接口仅1280新增参数，但完整训练32H200、实机20维动作，项目Code入口目前是占位。阅读88：适合理解视频预训练如何进入动作计算、训练分支与部署分支为何要一致，以及少步采样的条件。公开与评审按独立CoRL录用来源补齐；学术影响与近期关注按同日单篇计量另计。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 90.0 | 30% |
| 创新性 | 78 | 20% |
| 实验与证据 | 78 | 20% |
| 学术影响 | 0 | 10% |
| 近期关注 | 0 | 5% |
| 复用价值 | 65 | 8% |
| 阅读价值 | 88 | 7% |

刊会依据：[CoRL 2026](../../../venues/CoRL/README.md)，正式出处见[出版/原文记录](https://2026.corl.org/program/accepted-papers)；采用2026-10-10刊会快照。


公开与评审依据：v1完整公开且身份与版本可追溯；CoRL 2026官方录用表与原文首页确认录用，按既有CoRL 90分量表取较高阶段。；正式刊会按登记量表计分，取较高阶段。


编辑深度：阅读v1共22页主文及A–G相关附录，目视核Table1–3/6及采样图表，核动作patch形状、训练模式与推理条件；未执行代码复现，非完整公开精讲。；评分记录：2026-10-30。

计量来源：OpenAlex；arXiv v1; 10.48550/arXiv.2610.36823；匹配题目：TAPESTRY: A Single Backbone for Video Generation and Robot Control。累计被引 **0**，2025–2026 被引 **0**；快照：2026-10-30T13:51:43.624406+08:00。

[指标记录](https://api.openalex.org/works/https://doi.org/10.48550/arXiv.2610.36823) · [文献计量条目](https://openalex.org/W7224092217)

### 影响与关注的计算依据

- **学术影响 0**：OpenAlex精确DOI本次实测引用0；本次官方项目/作者/实验室/网页前5未定位独立技术采用，按量表起点0。目录收录与作者自述不算技术采用。 [依据1](https://arxiv.org/abs/2610.36823v1) · [依据2](https://arxiv.org/pdf/2610.36823v1) · [依据3](https://tapestry-wam.github.io/) · [依据4](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2610.36823?fields=title,authors,year,citationCount,influentialCitationCount,externalIds) · [依据5](https://api.openalex.org/works/https://doi.org/10.48550/arXiv.2610.36823) · [依据6](https://api.openalex.org/works?search=TAPESTRY%3A%20A%20Single%20Backbone%20for%20Video%20Generation%20and%20Robot%20Control&per-page=5) · [依据7](https://huggingface.co/api/papers/2610.36823)
- **近期关注 0**：匹配引用源当前0；HF单篇404，官方项目Code/#和arXiv/#，GitHub精确ID仓库检索无匹配；未取得单篇可核阅读/讨论/专属repo计数，按有来源量表起点0。未知平台指标仍null。 [依据1](https://arxiv.org/abs/2610.36823v1) · [依据2](https://arxiv.org/pdf/2610.36823v1) · [依据3](https://tapestry-wam.github.io/) · [依据4](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2610.36823?fields=title,authors,year,citationCount,influentialCitationCount,externalIds) · [依据5](https://api.openalex.org/works/https://doi.org/10.48550/arXiv.2610.36823) · [依据6](https://api.openalex.org/works?search=TAPESTRY%3A%20A%20Single%20Backbone%20for%20Video%20Generation%20and%20Robot%20Control&per-page=5) · [依据7](https://huggingface.co/api/papers/2610.36823)

零分表示本次快照已定位的信号处在量表起点；创新和实验两轴分别评价方法。

### 论文公开入口与传播快照

- [project 入口](https://tapestry-wam.github.io/)

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
