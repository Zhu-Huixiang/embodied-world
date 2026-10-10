# 3D Gaussian Splatting for Real-Time Radiance Field Rendering

**3DGS** · SIGGRAPH / TOG 2023 · 本版排名 10 · 综合分 **94.3 / 100**

[解读导读](../../../library/gaussian-splatting.md) · [具身感知与场景表示](../../../paper-map/README.md#track-embodied-perception) · [SIGGRAPH / TOG集锦](../../../venues/SIGGRAPH-TOG/README.md)

[原文](https://dl.acm.org/doi/10.1145/3592433) · [PDF](https://arxiv.org/pdf/2308.04079) · [阅读卡片](../../../library/gaussian-splatting.md)

论文出处：[**Bernhard Kerbl / Georgios Kopanas**](../../origins/papers/gaussian-splatting.md)<br>[法国 Inria 研究所 / 蔚蓝海岸大学 · 另1个机构](../../origins/papers/gaussian-splatting.md)

## 机制简析

从相机标定产生的稀疏点初始化三维高斯，优化位置、各向异性形状、不透明度与颜色。可微 splatting 渲染器把高斯投到图像平面，按可见性排序混合；训练中交替优化参数和增删高斯。原文比较多套真实场景的新视角质量、训练时间和渲染速度，后续机器人系统利用同类表示做语义掩码与场景编辑。

带着这个问题读：把神经场换成一群可编辑高斯，为什么渲染会快，场景操作又会方便在哪里？

初读判断：显式表示与高效渲染共同改变场景构建成本，标准场景对照充分，参考实现公开；CoRL 应用提供直接具身联系。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 90.4 | 30% |
| 创新性 | 95 | 20% |
| 实验与证据 | 93 | 20% |
| 学术影响 | 100 | 10% |
| 近期关注 | 100.0 | 5% |
| 复用价值 | 99 | 8% |
| 阅读价值 | 95 | 7% |

刊会依据：[SIGGRAPH / TOG 2023](../../../venues/SIGGRAPH-TOG/README.md)，正式出处见[出版/原文记录](https://dl.acm.org/doi/10.1145/3592433)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；正式刊会版本；匹配题目：3D Gaussian Splatting for Real-Time Radiance Field Rendering。累计被引 **5749**，2025–2026 被引 **4734**；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4385318467) · [文献计量条目](https://openalex.org/W4385318467)

### 影响与关注的计算依据

- **学术影响 100**：身份匹配的累计引用C=5749，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4385318467)
- **近期关注 100.0**：近期已定位引用R=4734；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W4385318467)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/graphdeco-inria/gaussian-splatting) | GitHub Star 24158；GitHub Watch订阅 155；GitHub Fork 3464 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2308.04079) | HF 论文累计点赞 205 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
