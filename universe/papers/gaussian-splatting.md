# 3DGS 星系

3D Gaussian Splatting for Real-Time Radiance Field Rendering

**导读** · 具身感知与场景表示

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/gaussian-splatting.md) · [原文](https://dl.acm.org/doi/10.1145/3592433) · [评分卡](../../leaderboard/papers/gaussian-splatting/README.md)

从相机标定产生的稀疏点初始化三维高斯，优化位置、各向异性形状、不透明度与颜色。可微 splatting 渲染器把高斯投到图像平面，按可见性排序混合；训练中交替优化参数和增删高斯。原文比较多套真实场景的新视角质量、训练时间和渲染速度，后续机器人系统利用同类表示做语义掩码与场景编辑。

## 技术挂点

- [新视角场景表示](../concepts/radiance.md)：从多视图学习场景的颜色、密度或高斯参数，通过渲染产生新的观察视角。

- [空间表示](../concepts/spatial.md)：保留像素、点、体素或对象相对位置的表示，让预测能接到几何与动作位置。

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。

## 本篇行星与卫星

- [新视角场景表示](gaussian-splatting/radiance.md) · 初读挂点
- [空间表示](gaussian-splatting/spatial.md) · 初读挂点
- [表征空间](gaussian-splatting/representation.md) · 初读挂点
- [本篇方法链路](gaussian-splatting/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
