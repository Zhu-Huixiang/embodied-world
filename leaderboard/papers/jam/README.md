# Vision-Language-Action or World-Action? Just Action Models

**JAM** · arXiv 2026 · 本版排名 110 · 综合分 **67.0 / 100**

[解读导读](../../../library/jam.md) · [视觉语言动作模型 VLA](../../../paper-map/README.md#track-vla) · [arXiv集锦](../../../arxiv/README.md#paper-jam)

[知识星系](../../../universe/papers/jam.md) · [原文](https://arxiv.org/abs/2610.37219v1) · [PDF](https://arxiv.org/pdf/2610.37219v1) · [阅读卡片](../../../library/jam.md)

论文出处：[**Yonghao Yu**](../../origins/papers/jam.md)<br>[东京大学 / 日本国立信息学研究所](../../origins/papers/jam.md)

## 机制简析

JAM把骨干初始化、未来监督和部署模块拆开：当前图像/语言经骨干提供视觉token，动作专家结合状态生成动作块。训练时，记录的未来只送入冻结anchor得到目标；一个额外prediction head从当前特征预测这些目标，以逐token/时间偏移的余弦距离加动作flow-matching损失训练，目标停止梯度。部署删除anchor和prediction head，动作路径不读未来，也不生成未来图像。固定未来目标可提前缓存；Wan配置以VAE直接编码目标最好，Ovis配置则用Yak特征，不能把结论简化成越大的未来模型越好。

带着这个问题读：VLA和WAM到底差在预训练起点，还是怎样利用未来？把未来监督留下、把视觉生成删掉，控制还会好吗？

初读判断：创新87：主要贡献是拆开三种设计选择并用可丢弃的未来表征预测统一两类骨干，未来预测本身有既有路线。证据88：两类骨干、固定LIBEROPlus子集、RoboTwin、七组目标/损失消融、任务bootstrap及三训练run互相支撑；控制评估仍是仿真，扰动类别并非全部提升。复用80：官方仓库提供训练/评估命令、十种recipe、checkpoint manifest和LIBERO权重入口，尚未执行复现；缓存有额外准备成本。阅读94：适合拆开“需要未来监督”与“必须生成未来画面”这两件事。影响与关注依逐篇外部证据另计。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 60 | 30% |
| 创新性 | 87 | 20% |
| 实验与证据 | 88 | 20% |
| 学术影响 | 0 | 10% |
| 近期关注 | 20.1 | 5% |
| 复用价值 | 80 | 8% |
| 阅读价值 | 94 | 7% |

公开与评审依据：arXiv v1完整公开，稳定身份、版本与作者可追溯，按公开阶段60计。；当前阶段为预印本公开。


编辑深度：arXiv v1主文方法/全部实验及Appendix A–E初读，非完整精讲；评分记录：2026-10-29。

累计引用与近期引用尚未匹配；原始值保留null。下面列出已定位的评分信号。

### 影响与关注的计算依据

- **学术影响 0**：本次有界补查未核到独立技术采用，按证据量表起点0；原始引用未匹配为null，非实测零引用。 [依据1](https://arxiv.org/abs/2610.37219v1) · [依据2](https://y0uroy.github.io/JAM/) · [依据3](https://api.semanticscholar.org/graph/v1/paper/ARXIV:2610.37219?fields=title,authors,year,externalIds,citationCount,citations.paperId,citations.year) · [依据4](https://api.openalex.org/works/https://doi.org/10.48550/arxiv.2610.37219) · [依据5](https://api.openalex.org/works?search=Vision-Language-Action+or+World-Action%3F+Just+Action+Models&per-page=5) · [依据6](https://huggingface.co/api/papers/2610.37219) · [依据7](https://api.github.com/search/repositories?q=2610.37219&per_page=10)
- **近期关注 20.1**：huggingface 的论文专属入口：HF论文点赞=3；按1000上限对数压缩。 [依据1](https://huggingface.co/api/papers/2610.37219) · [依据2](https://arxiv.org/abs/2610.37219v1) · [依据3](https://huggingface.co/papers/2610.37219)

零分表示本次快照已定位的信号处在量表起点；创新和实验两轴分别评价方法。

### 论文公开入口与传播快照

- [project 入口](https://y0uroy.github.io/JAM/)

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/y0urOy/JAM) | GitHub Star 2；GitHub Watch订阅 0；GitHub Fork 0 | 官方单篇代码仓库；截至2026-10-29的累计快照（近期新建入口） | 2026-10-29 |
| [huggingface](https://huggingface.co/papers/2610.37219) | HF论文点赞 3 | 精确arXiv ID单篇论文页；截至2026-10-29的累计快照（近期新建入口） | 2026-10-29 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
