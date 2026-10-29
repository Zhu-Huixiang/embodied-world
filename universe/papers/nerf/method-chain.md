# 本篇方法链路 · NeRF

给多层感知机输入三维位置与观察方向，输出体密度和视角相关颜色。沿每条相机射线查询多个点，体渲染把颜色与密度累积成像，再由多视角重建误差更新场景网络。位置编码保留高频细节，分层采样减少无效查询；原文比较真实与合成场景的新视角质量。

给多层感知机输入三维位置与观察方向，输出体密度和视角相关颜色。沿每条相机射线查询多个点，体渲染把颜色与密度累积成像，再由多视角重建误差更新场景网络。位置编码保留高频细节，分层采样减少无效查询；原文比较真实与合成场景的新视角质量。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/nerf-2003.08934/README.md#3-方法起点场景表示一个点为什么有两套答案)

[本篇星系](../nerf.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/nerf-2003.08934/README.md) · [原文依据](https://link.springer.com/chapter/10.1007/978-3-030-58452-8_24)
