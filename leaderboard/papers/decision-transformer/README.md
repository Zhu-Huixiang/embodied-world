# Decision Transformer: Reinforcement Learning via Sequence Modeling

**Decision Transformer** · NeurIPS 2021 · 本版排名 24 · 综合分 **90.2 / 100**

[解读导读](../../../library/decision-transformer.md) · [强化学习与离线决策](../../../paper-map/README.md#track-reinforcement-learning) · [NeurIPS集锦](../../../venues/NeurIPS/README.md)

[原文](https://proceedings.neurips.cc/paper_files/paper/2021/hash/7f489f642a0ddb10272b5c31057f0663-Abstract.html) · [PDF](https://proceedings.neurips.cc/paper_files/paper/2021/file/7f489f642a0ddb10272b5c31057f0663-Paper.pdf) · [阅读卡片](../../../library/decision-transformer.md)

论文出处：[Lili Chen / Kevin Lu · UC Berkeley / Meta FAIR 等3个出处](../../origins/papers/decision-transformer.md)

## 机制简析

把未来目标回报、状态和动作按时间交错成序列，因果 Transformer 用过去上下文预测当前动作。训练直接拟合数据动作；执行后减去已经获得的奖励，再把更新后的目标回报与新状态送回模型。实验用 Atari、Gym 与长时序任务检验这个条件生成式策略。

带着这个问题读：把目标回报放进 token 序列，就能把离线控制改写成条件生成吗？

初读判断：方法提出清晰的新决策表述，正式论文跨离散与连续域，后续 Trajectory Transformer 对其优缺点作直接比较。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 95 | 20% |
| 实验与证据 | 84 | 20% |
| 学术影响 | 76.6 | 10% |
| 近期关注 | 76.0 | 5% |
| 复用价值 | 95 | 8% |
| 阅读价值 | 97 | 7% |

刊会依据：[NeurIPS 2021](../../../venues/NeurIPS/README.md)，正式出处见[出版/原文记录](https://proceedings.neurips.cc/paper_files/paper/2021/hash/7f489f642a0ddb10272b5c31057f0663-Abstract.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本/原研究索引记录；匹配题目：Decision Transformer: Reinforcement Learning via Sequence Modeling。累计被引 **459**，2025–2026 被引 **89**；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W3169291081) · [文献计量条目](https://openalex.org/W3169291081)

### 影响与关注的计算依据

- **学术影响 76.6**：身份匹配的累计引用C=459，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W3169291081)
- **近期关注 76.0**：huggingface 的论文专属入口：HF 最近30天下载=6309；按100000上限对数压缩。 [依据1](https://huggingface.co/api/models/edbeeching/decision-transformer-gym-hopper-medium) · [依据2](https://huggingface.co/edbeeching/decision-transformer-gym-hopper-medium/raw/main/README.md) · [依据3](https://huggingface.co/edbeeching/decision-transformer-gym-hopper-medium)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [huggingface](https://huggingface.co/edbeeching/decision-transformer-gym-hopper-medium) | HF 最近30天下载 6309；HF 仓库累计点赞 7 | 单篇论文的第三方实现/数据格式转换，按此仓库统计；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2106.01345) | HF 论文累计点赞 4 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
