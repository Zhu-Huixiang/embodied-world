# NeRF: Representing Scenes as Neural Radiance Fields for View Synthesis

**解读导读** · ECCV 2020 · [具身感知与场景表示](../paper-map/README.md#track-embodied-perception)

研究范围：生成/表征基础，机器人场景重建、特征场与视觉仿真的连续场表示。

[原文入口](https://link.springer.com/chapter/10.1007/978-3-030-58452-8_24) · [原文 PDF](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123460392.pdf) · [作者项目 / 代码入口](https://www.matthewtancik.com/nerf) · [作者与团队](../leaderboard/origins/papers/nerf.md)

ECCV 2020 原始论文；作者项目注明 ECCV 2020 Oral，原文实验是新视角合成。

## 先看它做了什么

给多层感知机输入三维位置与观察方向，输出体密度和视角相关颜色。沿每条相机射线查询多个点，体渲染把颜色与密度累积成像，再由多视角重建误差更新场景网络。位置编码保留高频细节，分层采样减少无效查询；原文比较真实与合成场景的新视角质量。

## 带着什么问题读

**多张照片怎样变成可以换视角查看的场景，射线上每个采样点算了什么？**

## 为什么值得继续读

神经辐射场成为后续语义特征场和机器人操作地图的基础；Splat-MOVER 相关工作直接描述 NeRF 型 LERF-TOGO/F3RM 链路。

证据入口：表示、渲染和监督链路具有奠基价值，标准数据集对照明确，作者代码公开；后续机器人场景表示用途有公开机器人论文支撑。

具身关联：神经辐射场成为后续语义特征场和机器人操作地图的基础；Splat-MOVER 相关工作直接描述 NeRF 型 LERF-TOGO/F3RM 链路。

经典保留理由：2020 年经典例外：连续场、体渲染和可微场景拟合是后来机器人三维特征场与场景重建的重要起点。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/nerf/README.md) · [ECCV集锦](../venues/ECCV/README.md) · [地图方向](../paper-map/README.md#track-embodied-perception) · [首页](../README.md)

元数据核对：2026-10-10。
