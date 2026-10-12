# NeRF 星系

NeRF: Representing Scenes as Neural Radiance Fields for View Synthesis

**导读** · 具身感知与场景表示

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/nerf.md) · [原文](https://link.springer.com/chapter/10.1007/978-3-030-58452-8_24) · [评分卡](../../leaderboard/papers/nerf/README.md)

给多层感知机输入三维位置与观察方向，输出体密度和视角相关颜色。沿每条相机射线查询多个点，体渲染把颜色与密度累积成像，再由多视角重建误差更新场景网络。位置编码保留高频细节，分层采样减少无效查询；原文比较真实与合成场景的新视角质量。

## 技术挂点

- [新视角场景表示](../concepts/radiance.md)：从多视图学习场景的颜色、密度或高斯参数，通过渲染产生新的观察视角。

- [空间表示](../concepts/spatial.md)：保留像素、点、体素或对象相对位置的表示，让预测能接到几何与动作位置。

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。

## 本篇行星与卫星

- [新视角场景表示](nerf/radiance.md) · 初读挂点
- [空间表示](nerf/spatial.md) · 初读挂点
- [表征空间](nerf/representation.md) · 初读挂点
- [本篇方法链路](nerf/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
