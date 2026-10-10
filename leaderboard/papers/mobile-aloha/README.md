# Mobile ALOHA: Learning Bimanual Mobile Manipulation using Low-Cost Whole-Body Teleoperation

**Mobile ALOHA** · CoRL 2024 · 本版排名 70 · 综合分 **84.1 / 100**

[解读导读](../../../library/mobile-aloha.md) · [操作与动作块](../../../paper-map/README.md#track-manipulation) · [CoRL集锦](../../../venues/CoRL/README.md)

[原文](https://proceedings.mlr.press/v270/fu25b.html) · [PDF](https://raw.githubusercontent.com/mlresearch/v270/main/assets/fu25b/fu25b.pdf) · [阅读卡片](../../../library/mobile-aloha.md)

论文出处：[Zipeng Fu · Stanford University](../../origins/papers/mobile-aloha.md)

## 机制简析

把双臂关节位置与底盘线/角速度拼成统一动作，遥操作同时记录手臂与底盘；行为克隆直接预测整套动作。训练混入已有静态 ALOHA 示范，检验不同任务、臂安装位置和场景之间的正迁移。原文把自治策略执行与人类遥操作采集分开，比较联合训练和只用移动数据的任务表现。

带着这个问题读：桌面双臂经验为什么能帮会移动的机器人做饭、开柜子和坐电梯？

初读判断：CoRL 正式稿与首版方法给出真实长程移动任务和联合训练对照，开放软硬件便于复用；视觉演示具有传播价值，评分仍以自治任务评估而非视频震撼程度为依据。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 90.0 | 30% |
| 创新性 | 87 | 20% |
| 实验与证据 | 90 | 20% |
| 学术影响 | 42.9 | 10% |
| 近期关注 | 63.7 | 5% |
| 复用价值 | 93 | 8% |
| 阅读价值 | 97 | 7% |

刊会依据：[CoRL 2024](../../../venues/CoRL/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v270/fu25b.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本/原研究索引记录；匹配题目：Mobile ALOHA: Learning Bimanual Mobile Manipulation with Low-Cost Whole-Body Teleoperation。累计被引 **30**，2025–2026 被引 **15**；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4390635563) · [文献计量条目](https://openalex.org/W4390635563)

### 影响与关注的计算依据

- **学术影响 42.9**：身份匹配的累计引用C=30，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4390635563)
- **近期关注 63.7**：huggingface 的论文专属入口：HF 最近30天下载=1532；按100000上限对数压缩。 [依据1](https://huggingface.co/api/datasets/lerobot/aloha_mobile_wipe_wine) · [依据2](https://huggingface.co/datasets/lerobot/aloha_mobile_wipe_wine/raw/main/README.md) · [依据3](https://huggingface.co/datasets/lerobot/aloha_mobile_wipe_wine)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/MarkFzp/act-plus-plus) | GitHub Star 3669；GitHub Watch订阅 47；GitHub Fork 649 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [github](https://github.com/MarkFzp/mobile-aloha) | GitHub Star 4473；GitHub Watch订阅 78；GitHub Fork 732 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/datasets/lerobot/aloha_mobile_wipe_wine) | HF 最近30天下载 1532；HF 仓库累计点赞 3 | 单篇论文的第三方实现/数据格式转换，按此仓库统计；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2401.02117) | HF 论文累计点赞 33 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
