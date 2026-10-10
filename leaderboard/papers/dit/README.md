# Scalable Diffusion Models with Transformers

**DiT** · ICCV 2023 · 本版排名 11 · 综合分 **94.2 / 100**

[解读导读](../../../library/dit.md) · [Diffusion / Transformer 基础](../../../paper-map/README.md#track-diffusion-transformer) · [ICCV集锦](../../../venues/ICCV/README.md)

[原文](https://openaccess.thecvf.com/content/ICCV2023/html/Peebles_Scalable_Diffusion_Models_with_Transformers_ICCV_2023_paper.html) · [PDF](https://openaccess.thecvf.com/content/ICCV2023/papers/Peebles_Scalable_Diffusion_Models_with_Transformers_ICCV_2023_paper.pdf) · [阅读卡片](../../../library/dit.md)

## 机制简析

在图像潜表示的patch序列上用Transformer做扩散去噪，考察计算规模和条件注入。

带着这个问题读：Transformer 怎样在潜空间去噪，条件又怎样进入各层？

初读判断：生成架构影响力和实现复用突出；作为视频/动作模型前置，保留图像任务范围。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 95.0 | 30% |
| 创新性 | 95 | 20% |
| 实验与证据 | 91 | 20% |
| 学术影响 | 95.3 | 10% |
| 近期关注 | 100 | 5% |
| 复用价值 | 94 | 8% |
| 阅读价值 | 92 | 7% |

刊会依据：[ICCV 2023](../../../venues/ICCV/README.md)，正式出处见[出版/原文记录](https://openaccess.thecvf.com/content/ICCV2023/html/Peebles_Scalable_Diffusion_Models_with_Transformers_ICCV_2023_paper.html)；采用2026-10-10刊会快照。


编辑深度：选题初读；评分记录：2026-10-10。

计量版本：正式刊会版本；OpenAlex题目：Scalable Diffusion Models with Transformers。累计被引 2065，2025–2026 被引 1742；快照：2026-10-09T18:35:28+08:00。

[指标记录](https://api.openalex.org/works/W4390872297) · [文献计量条目](https://openalex.org/W4390872297)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
