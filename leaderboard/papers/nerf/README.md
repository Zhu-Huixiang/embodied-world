# NeRF: Representing Scenes as Neural Radiance Fields for View Synthesis

**NeRF** · ECCV 2020 · 本版排名 13 · 综合分 **92.4 / 100**

[解读导读](../../../library/nerf.md) · [具身感知与场景表示](../../../paper-map/README.md#track-embodied-perception) · [ECCV集锦](../../../venues/ECCV/README.md)

[原文](https://link.springer.com/chapter/10.1007/978-3-030-58452-8_24) · [PDF](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123460392.pdf) · [阅读卡片](../../../library/nerf.md)

论文出处：[**Ben Mildenhall**](../../origins/papers/nerf.md)<br>[加州大学伯克利分校 / 谷歌研究院 · 另1个机构](../../origins/papers/nerf.md)

## 机制简析

给多层感知机输入三维位置与观察方向，输出体密度和视角相关颜色。沿每条相机射线查询多个点，体渲染把颜色与密度累积成像，再由多视角重建误差更新场景网络。位置编码保留高频细节，分层采样减少无效查询；原文比较真实与合成场景的新视角质量。

带着这个问题读：多张照片怎样变成可以换视角查看的场景，射线上每个采样点算了什么？

初读判断：表示、渲染和监督链路具有奠基价值，标准数据集对照明确，作者代码公开；后续机器人场景表示用途有公开机器人论文支撑。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 83.0 | 30% |
| 创新性 | 97 | 20% |
| 实验与证据 | 93 | 20% |
| 学术影响 | 100 | 10% |
| 近期关注 | 100.0 | 5% |
| 复用价值 | 98 | 8% |
| 阅读价值 | 95 | 7% |

刊会依据：[ECCV 2020](../../../venues/ECCV/README.md)，正式出处见[出版/原文记录](https://link.springer.com/chapter/10.1007/978-3-030-58452-8_24)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；正式刊会版本；匹配题目：NeRF: Representing Scenes as Neural Radiance Fields for View Synthesis。累计被引 **5156**，2025–2026 被引 **1759**；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W3109585842) · [文献计量条目](https://openalex.org/W3109585842)

### 影响与关注的计算依据

- **学术影响 100**：身份匹配的累计引用C=5156，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W3109585842)
- **近期关注 100.0**：近期已定位引用R=1759；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W3109585842)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/bmild/nerf) | GitHub Star 10945；GitHub Watch订阅 133；GitHub Fork 1426 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2003.08934) | HF 论文累计点赞 2 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
