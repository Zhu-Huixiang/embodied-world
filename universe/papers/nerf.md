# NeRF 星系

NeRF: Representing Scenes as Neural Radiance Fields for View Synthesis

**已精讲** · 具身感知与场景表示

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/nerf-2003.08934/README.md) · [原文](https://link.springer.com/chapter/10.1007/978-3-030-58452-8_24) · [评分卡](../../leaderboard/papers/nerf/README.md)

给多层感知机输入三维位置与观察方向，输出体密度和视角相关颜色。沿每条相机射线查询多个点，体渲染把颜色与密度累积成像，再由多视角重建误差更新场景网络。位置编码保留高频细节，分层采样减少无效查询；原文比较真实与合成场景的新视角质量。

## 技术挂点

- [新视角场景表示](../concepts/radiance.md)：从多视图学习场景的颜色、密度或高斯参数，通过渲染产生新的观察视角。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/nerf-2003.08934/README.md#31-位置定密度方向管反光)

- [空间表示](../concepts/spatial.md)：保留像素、点、体素或对象相对位置的表示，让预测能接到几何与动作位置。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/nerf-2003.08934/README.md#2-相关工作表面体素与连续函数)

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/nerf-2003.08934/README.md#32-mlp-里面到底走了几步)

## 本篇行星与卫星

- [新视角场景表示](nerf/radiance.md) · 已讲解
- [空间表示](nerf/spatial.md) · 已讲解
- [表征空间](nerf/representation.md) · 已讲解
- [本篇方法链路](nerf/method-chain.md) · 已讲解
- [场景专属连续函数](nerf/scene-function.md) · 已讲解
- [表面与体积表示](nerf/surface-volume.md) · 已讲解
- [体密度](nerf/density.md) · 已讲解
- [方向相关颜色](nerf/view-color.md) · 已讲解
- [单位方向自由度](nerf/unit-direction.md) · 已讲解
- [密度颜色分支](nerf/mlp-branch.md) · 已讲解
- [输入跳接](nerf/skip-input.md) · 已讲解
- [像素射线](nerf/camera-ray.md) · 已讲解
- [累积透射](nerf/transmittance.md) · 已讲解
- [前向alpha合成](nerf/alpha-composite.md) · 已讲解
- [分层随机采样](nerf/stratified.md) · 已讲解
- [正弦余弦坐标编码](nerf/fourier-coordinates.md) · 已讲解
- [低频拟合偏好](nerf/spectral-bias.md) · 已讲解
- [粗细网络采样](nerf/coarse-fine.md) · 已讲解
- [逆CDF采样](nerf/inverse-cdf.md) · 已讲解
- [像素监督与可微渲染](nerf/rgb-supervision.md) · 已讲解
- [相机标定与COLMAP](nerf/camera-calibration.md) · 已讲解
- [归一化设备坐标](nerf/ndc.md) · 已讲解
- [新视角质量指标](nerf/quality-metrics.md) · 已讲解
- [表示与采样消融](nerf/ablation-components.md) · 已讲解
- [存储计算交换](nerf/runtime-budget.md) · 已讲解

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
