# VideoVLA: Video Generators Can Be Generalizable Robot Manipulators

**VideoVLA** · NeurIPS 2025 · 本版排名 102 · 综合分 **78.8 / 100**

[解读导读](../../../library/videovla.md) · [视频动作模型与视觉推理](../../../paper-map/README.md#track-video-action) · [NeurIPS集锦](../../../venues/NeurIPS/README.md)

[原文](https://proceedings.neurips.cc/paper_files/paper/2025/hash/89a3b655a8b68ae1c76b768152c9c19d-Abstract-Conference.html) · [PDF](https://proceedings.neurips.cc/paper_files/paper/2025/file/89a3b655a8b68ae1c76b768152c9c19d-Paper-Conference.pdf) · [阅读卡片](../../../library/videovla.md)

论文出处：[Yichao Shen · IAIR, Xi’an Jiaotong University / Microsoft Research Asia (China) 等3个出处](../../origins/papers/videovla.md)

## 机制简析

以视频生成器的时空动态先验联合预测未来画面与机器人动作，考察未见操作泛化。

带着这个问题读：视频生成先验怎样与动作预测一起用于操作泛化？

初读判断：未来视觉与动作的对应关系值得拆；按正式NeurIPS原作范围阅读。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 88 | 20% |
| 实验与证据 | 82 | 20% |
| 学术影响 | 17.3 | 10% |
| 近期关注 | 38.0 | 5% |
| 复用价值 | 80 | 8% |
| 阅读价值 | 90 | 7% |

刊会依据：[NeurIPS 2025](../../../venues/NeurIPS/README.md)，正式出处见[出版/原文记录](https://proceedings.neurips.cc/paper_files/paper/2025/hash/89a3b655a8b68ae1c76b768152c9c19d-Abstract-Conference.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：选题初读；评分记录：2026-10-10。

计量来源：OpenAlex；正式刊会版本；匹配题目：VideoVLA: Video Generators Can Be Generalizable Robot Manipulators。累计被引 **3**，2025–2026 被引 **3**；快照：2026-10-09T18:35:28+08:00。

[指标记录](https://api.openalex.org/works/W7196952124) · [文献计量条目](https://openalex.org/W7196952124)

### 影响与关注的计算依据

- **学术影响 17.3**：身份匹配的累计引用C=3，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W7196952124)
- **近期关注 38.0**：近期窗口内创建的专属论文仓库，快照star=32；按10000上限对数压缩。 [依据1](https://api.github.com/repos/VideoVLA-Project/VideoVLA) · [依据2](https://raw.githubusercontent.com/VideoVLA-Project/VideoVLA/main/README.md)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/VideoVLA-Project/VideoVLA) | GitHub Star 32；GitHub Watch订阅 0；GitHub Fork 4 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/VideoVLA/VideoVLA_Cogvideobase_Pretrained) | HF 最近30天下载 0；HF 仓库累计点赞 0 | 单篇论文的作者发布资产；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2512.06963) | HF 论文累计点赞 5 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
