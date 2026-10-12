# 空间表示

保留像素、点、体素或对象相对位置的表示，让预测能接到几何与动作位置。

全局语义向量识别杯子；抓哪里还需要空间接口。

分类上层：[表征空间](representation.md)。

继续拆：[点云与三维体素](point-cloud.md) · [新视角场景表示](radiance.md)。

## 在完整解读里看计算与例子

- [CLIP：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#6-局限认出杯子距离抓住杯子还差什么)

## 哪些论文用到或讨论它

- [Perceptive Locomotion](../papers/perceptive-loco.md) · 机制导读 · [原文](https://www.science.org/doi/10.1126/scirobotics.abk2822)
- [Agile Flight](../papers/agile-flight.md) · 机制导读 · [原文](https://www.science.org/doi/10.1126/scirobotics.abg5810)
- [CLIPort](../papers/cliport.md) · 机制导读 · [原文](https://proceedings.mlr.press/v164/shridhar22a.html)
- [PerAct](../papers/peract.md) · 机制导读 · [原文](https://proceedings.mlr.press/v205/shridhar23a.html)
- [RVT](../papers/rvt.md) · 机制导读 · [原文](https://proceedings.mlr.press/v229/goyal23a.html)
- [RVT-2](../papers/rvt2.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss20/p055.html)
- [Transporter](../papers/transporter.md) · 机制导读 · [原文](https://proceedings.mlr.press/v155/zeng21a.html)
- [ANYmal Parkour](../papers/anymal-parkour.md) · 机制导读 · [原文](https://www.science.org/doi/10.1126/scirobotics.adi7566)
- [CLIP](../papers/clip.md) · 已精讲 · [原文](https://proceedings.mlr.press/v139/radford21a.html)
- [SAM](../papers/sam.md) · 机制导读 · [原文](https://openaccess.thecvf.com/content/ICCV2023/html/Kirillov_Segment_Anything_ICCV_2023_paper.html)
- [SAM 2](../papers/sam2.md) · 机制导读 · [原文](https://openreview.net/forum?id=Ha6RTeWMd0)
- [NeRF](../papers/nerf.md) · 机制导读 · [原文](https://link.springer.com/chapter/10.1007/978-3-030-58452-8_24)
- [3DGS](../papers/gaussian-splatting.md) · 机制导读 · [原文](https://dl.acm.org/doi/10.1145/3592433)
- [Dynamics Review](../papers/learned-dynamics-review.md) · 机制导读 · [原文](https://www.science.org/doi/10.1126/scirobotics.adt1497)
- [Dex-One2Many](../papers/dex-one2many.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.12470v1)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
