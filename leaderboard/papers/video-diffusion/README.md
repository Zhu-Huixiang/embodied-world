# Video Diffusion Models

**Video Diffusion** · NeurIPS 2022 · 本版排名 29 · 综合分 **89.2 / 100**

[解读导读](../../../library/video-diffusion.md) · [视频与序列生成](../../../paper-map/README.md#track-video-generation) · [NeurIPS集锦](../../../venues/NeurIPS/README.md)

[原文](https://proceedings.neurips.cc/paper_files/paper/2022/hash/39235c56aef13fb05a6adc95eb9d8d66-Abstract-Conference.html) · [PDF](https://proceedings.neurips.cc/paper_files/paper/2022/file/39235c56aef13fb05a6adc95eb9d8d66-Paper-Conference.pdf) · [阅读卡片](../../../library/video-diffusion.md)

论文出处：[**Jonathan Ho**](../../origins/papers/video-diffusion.md)<br>[谷歌研究院](../../origins/papers/video-diffusion.md)

## 机制简析

把图像扩散 U-Net 扩成空间与时间分解的网络，空间卷积处理每帧内容，时间注意力在对应位置之间传信息。图像与视频联合训练共享视觉能力，再以条件采样扩展时间和空间范围。原文在视频预测、无条件视频与文本条件视频任务比较生成质量和时序一致性。

带着这个问题读：逐帧画图为什么会抖，空间与时间注意力怎样让一段未来视频连起来？

初读判断：时空结构和联合训练的设计明确，跨生成任务有原始对照；作者演示公开，复用分低于完整开放训练权重的基础项目。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 91 | 20% |
| 实验与证据 | 91 | 20% |
| 学术影响 | 67.6 | 10% |
| 近期关注 | 74.0 | 5% |
| 复用价值 | 89 | 8% |
| 阅读价值 | 96 | 7% |

刊会依据：[NeurIPS 2022](../../../venues/NeurIPS/README.md)，正式出处见[出版/原文记录](https://proceedings.neurips.cc/paper_files/paper/2022/hash/39235c56aef13fb05a6adc95eb9d8d66-Abstract-Conference.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；正式刊会版本；匹配题目：Video Diffusion Models。累计被引 **223**，2025–2026 被引 **217**；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W7133218093) · [文献计量条目](https://openalex.org/W7133218093)

### 影响与关注的计算依据

- **学术影响 67.6**：身份匹配的累计引用C=223，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W7133218093)
- **近期关注 74.0**：近期已定位引用R=217；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W7133218093)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [huggingface](https://huggingface.co/papers/2204.03458) | HF 论文累计点赞 5 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
