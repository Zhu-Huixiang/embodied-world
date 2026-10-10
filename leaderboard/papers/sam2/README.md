# SAM 2: Segment Anything in Images and Videos

**SAM 2** · ICLR 2025 · 本版排名 17 · 综合分 **91.2 / 100**

[解读导读](../../../library/sam2.md) · [具身感知与场景表示](../../../paper-map/README.md#track-embodied-perception) · [ICLR集锦](../../../venues/ICLR/README.md)

[原文](https://openreview.net/forum?id=Ha6RTeWMd0) · [PDF](https://proceedings.iclr.cc/paper_files/paper/2025/file/45c1f6a8cbf2da59ebf2c802b4f742cd-Paper-Conference.pdf) · [阅读卡片](../../../library/sam2.md)

论文出处：[Nikhila Ravi · Meta FAIR](../../origins/papers/sam2.md)

## 机制简析

逐帧图像特征通过记忆注意力读取之前的目标提示与掩码信息，再与当前提示一起预测本帧掩码。记忆编码器把当前预测存入记忆，下一帧继续使用；静态图像相当于记忆为空的视频。原文比较交互次数、速度以及图像和视频分割基准。

带着这个问题读：目标在机器人视野里移动、遮挡后重现，过去的掩码记忆怎样帮它跟住对象？

初读判断：流式记忆和对象持续性问题直接，跨数据集与交互成本评估较完整，代码、模型及视频分割数据公开。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 87 | 20% |
| 实验与证据 | 95 | 20% |
| 学术影响 | 69.7 | 10% |
| 近期关注 | 100 | 5% |
| 复用价值 | 98 | 8% |
| 阅读价值 | 92 | 7% |

刊会依据：[ICLR 2025](../../../venues/ICLR/README.md)，正式出处见[出版/原文记录](https://openreview.net/forum?id=Ha6RTeWMd0)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本/原研究索引记录；匹配题目：SAM 2: Segment Anything in Images and Videos。累计被引 **264**，2025–2026 被引 **249**；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4401307635) · [文献计量条目](https://openalex.org/W4401307635)

### 影响与关注的计算依据

- **学术影响 69.7**：身份匹配的累计引用C=264，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4401307635)
- **近期关注 100**：huggingface 的论文专属入口：HF 最近30天下载=140043；按100000上限对数压缩。 [依据1](https://huggingface.co/api/models/facebook/sam2-hiera-base-plus) · [依据2](https://huggingface.co/facebook/sam2-hiera-base-plus/raw/main/README.md) · [依据3](https://huggingface.co/facebook/sam2-hiera-base-plus)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/facebookresearch/sam2) | GitHub Star 19977；GitHub Watch订阅 113；GitHub Fork 2568 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/facebook/sam2-hiera-base-plus) | HF 最近30天下载 140043；HF 仓库累计点赞 15 | 单篇原研究权重的HF转换版，按此仓库统计；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2408.00714) | HF 论文累计点赞 123 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
