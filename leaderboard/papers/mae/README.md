# Masked Autoencoders Are Scalable Vision Learners

本版阅读优先顺序：5；综合分：95.3 / 100；已评分权重：100%。

[原文](https://openaccess.thecvf.com/content/CVPR2022/html/He_Masked_Autoencoders_Are_Scalable_Vision_Learners_CVPR_2022_paper.html) · [PDF](https://openaccess.thecvf.com/content/CVPR2022/papers/He_Masked_Autoencoders_Are_Scalable_Vision_Learners_CVPR_2022_paper.pdf) · [阅读卡片](../../../library/mae.md)

## 机制简析

随机遮住大部分图像 patch，编码器只处理可见部分，轻量解码器再接入 mask token 还原缺失像素。非对称结构减少昂贵编码器的计算，高遮挡比例让补全任务需要理解物体和场景。原文比较分类、检测、分割迁移；MVP 将同类编码器冻结后接到可训练控制模块。

带着这个问题读：遮住四分之三的图像后还原像素，怎样帮助机器人把预训练视觉特征用于控制？

初读判断：方法和计算节省能直接从结构理解，视觉迁移实验完整，官方实现公开；机器人实机继承关系有 MVP 原文佐证。

## 七维评分

![七维雷达：加载时展开一次，随后静止](radar.gif)

打开时从中心展开一次，结束后保持最终形状。[直接查看静态图](radar.svg)。加载与再次打开的播放时机取决于浏览器缓存。

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 刊会质量 | 95.0 | 30% |
| 创新性 | 91 | 20% |
| 实验与证据 | 95 | 20% |
| 学术影响 | 100 | 10% |
| 近期关注 | 100 | 5% |
| 复用价值 | 98 | 8% |
| 阅读价值 | 96 | 7% |

刊会依据：[CVPR 2022](../../../venues/CVPR/README.md)，正式出处见[出版/原文记录](https://openaccess.thecvf.com/content/CVPR2022/html/He_Masked_Autoencoders_Are_Scalable_Vision_Learners_CVPR_2022_paper.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：正式刊会版本；OpenAlex题目：Masked Autoencoders Are Scalable Vision Learners。累计被引 7952，2025–2026 被引 3761；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4226002507) · [文献计量条目](https://openalex.org/W4226002507)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
