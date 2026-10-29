# 新视角场景表示

从多视图学习场景的颜色、密度或高斯参数，通过渲染产生新的观察视角。

NeRF 查询场景函数；3D Gaussian Splatting 投影混合高斯。

分类上层：[空间表示](spatial.md)。

## 在完整解读里看计算与例子

- [3DGS：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/gaussian-splatting-2308.04079/README.md#3-总览照片怎样变成可渲染的场景)
- [NeRF：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/nerf-2003.08934/README.md#31-位置定密度方向管反光)

## 哪些论文用到或讨论它

- [NeRF](../papers/nerf.md) · 已精讲 · [原文](https://link.springer.com/chapter/10.1007/978-3-030-58452-8_24)
- [3DGS](../papers/gaussian-splatting.md) · 已精讲 · [原文](https://dl.acm.org/doi/10.1145/3592433)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
