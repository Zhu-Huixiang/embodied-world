# 3DGS 星系

3D Gaussian Splatting for Real-Time Radiance Field Rendering

**已精讲** · 具身感知与场景表示

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/gaussian-splatting-2308.04079/README.md) · [原文](https://dl.acm.org/doi/10.1145/3592433) · [评分卡](../../leaderboard/papers/gaussian-splatting/README.md)

从相机标定产生的稀疏点初始化三维高斯，优化位置、各向异性形状、不透明度与颜色。可微 splatting 渲染器把高斯投到图像平面，按可见性排序混合；训练中交替优化参数和增删高斯。原文比较多套真实场景的新视角质量、训练时间和渲染速度，后续机器人系统利用同类表示做语义掩码与场景编辑。

## 技术挂点

- [新视角场景表示](../concepts/radiance.md)：从多视图学习场景的颜色、密度或高斯参数，通过渲染产生新的观察视角。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/gaussian-splatting-2308.04079/README.md#3-总览照片怎样变成可渲染的场景)

- [空间表示](../concepts/spatial.md)：保留像素、点、体素或对象相对位置的表示，让预测能接到几何与动作位置。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/gaussian-splatting-2308.04079/README.md#41-b-区一个高斯不是一颗固定圆球)

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/gaussian-splatting-2308.04079/README.md#41-b-区一个高斯不是一颗固定圆球)

## 本篇行星与卫星

- [新视角场景表示](gaussian-splatting/radiance.md) · 已讲解
- [空间表示](gaussian-splatting/spatial.md) · 已讲解
- [表征空间](gaussian-splatting/representation.md) · 已讲解
- [本篇方法链路](gaussian-splatting/method-chain.md) · 初读挂点
- [静态场景新视角](gaussian-splatting/novel-view.md) · 已讲解
- [SfM初始化](gaussian-splatting/sfm.md) · 已讲解
- [可优化三维高斯](gaussian-splatting/gaussian.md) · 已讲解
- [各向异性尺度旋转](gaussian-splatting/anisotropic.md) · 已讲解
- [投影协方差](gaussian-splatting/projection.md) · 已讲解
- [球谐方向颜色](gaussian-splatting/sh.md) · 已讲解
- [透明度与alpha](gaussian-splatting/alpha.md) · 已讲解
- [前向透明度合成](gaussian-splatting/composite.md) · 已讲解
- [像素与结构损失](gaussian-splatting/loss.md) · 已讲解
- [自适应密度控制](gaussian-splatting/densify.md) · 已讲解
- [复制小高斯](gaussian-splatting/clone.md) · 已讲解
- [拆分大高斯](gaussian-splatting/split.md) · 已讲解
- [修剪和透明度重置](gaussian-splatting/prune.md) · 已讲解
- [分块复制与排序](gaussian-splatting/tiles.md) · 已讲解
- [前向早停](gaussian-splatting/early-stop.md) · 已讲解
- [反向重走列表](gaussian-splatting/backward.md) · 已讲解
- [画质速度内存三本账](gaussian-splatting/metrics.md) · 已讲解
- [密度与形状消融](gaussian-splatting/ablation.md) · 已讲解
- [外观与物理分界](gaussian-splatting/robot-boundary.md) · 已讲解

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
