# Emerging Properties in Self-Supervised Vision Transformers

**DINO** · ICCV 2021 · 本版排名 9 · 综合分 **94.3 / 100**

[解读导读](../../../library/dino.md) · [具身感知与场景表示](../../../paper-map/README.md#track-embodied-perception) · [ICCV集锦](../../../venues/ICCV/README.md)

[原文](https://openaccess.thecvf.com/content/ICCV2021/html/Caron_Emerging_Properties_in_Self-Supervised_Vision_Transformers_ICCV_2021_paper.html) · [PDF](https://openaccess.thecvf.com/content/ICCV2021/papers/Caron_Emerging_Properties_in_Self-Supervised_Vision_Transformers_ICCV_2021_paper.pdf) · [阅读卡片](../../../library/dino.md)

## 机制简析

同一图像的不同裁剪分别进入学生和教师，学生用交叉熵拟合教师输出的概率分布。教师参数由学生参数的指数滑动平均更新，中心化与温度锐化防止两者退化成常量。原文比较 ViT 与卷积网络，检查 k-NN、线性分类和注意力中出现的物体区域结构。

带着这个问题读：没有人工标签，教师与学生互相对齐怎么还能长出物体边界？

初读判断：动量教师、裁剪与防坍塌措施能逐项分析，视觉迁移和空间结构有原始实验支撑，官方实现可复用。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 95.0 | 30% |
| 创新性 | 93 | 20% |
| 实验与证据 | 90 | 20% |
| 学术影响 | 100 | 10% |
| 近期关注 | 100 | 5% |
| 复用价值 | 96 | 8% |
| 阅读价值 | 93 | 7% |

刊会依据：[ICCV 2021](../../../venues/ICCV/README.md)，正式出处见[出版/原文记录](https://openaccess.thecvf.com/content/ICCV2021/html/Caron_Emerging_Properties_in_Self-Supervised_Vision_Transformers_ICCV_2021_paper.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：正式刊会版本；OpenAlex题目：Emerging Properties in Self-Supervised Vision Transformers。累计被引 5634，2025–2026 被引 2664；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W3159481202) · [文献计量条目](https://openalex.org/W3159481202)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
