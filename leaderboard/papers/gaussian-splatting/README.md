# 3D Gaussian Splatting for Real-Time Radiance Field Rendering

**3DGS** · SIGGRAPH / TOG 2023 · 本版排名 10 · 综合分 **94.3 / 100**

[原文](https://dl.acm.org/doi/10.1145/3592433) · [PDF](https://arxiv.org/pdf/2308.04079) · [阅读卡片](../../../library/gaussian-splatting.md)

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
| 发表与刊会 | 90.4 | 30% |
| 创新性 | 95 | 20% |
| 实验与证据 | 93 | 20% |
| 学术影响 | 100 | 10% |
| 近期关注 | 100 | 5% |
| 复用价值 | 99 | 8% |
| 阅读价值 | 95 | 7% |

刊会依据：[SIGGRAPH / TOG 2023](../../../venues/SIGGRAPH-TOG/README.md)，正式出处见[出版/原文记录](https://dl.acm.org/doi/10.1145/3592433)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：正式刊会版本；OpenAlex题目：3D Gaussian Splatting for Real-Time Radiance Field Rendering。累计被引 5749，2025–2026 被引 4734；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4385318467) · [文献计量条目](https://openalex.org/W4385318467)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
