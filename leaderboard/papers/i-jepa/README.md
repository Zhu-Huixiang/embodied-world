# Self-Supervised Learning from Images with a Joint-Embedding Predictive Architecture

**I-JEPA** · CVPR 2023 · 本版排名 25 · 综合分 **90.1 / 100**

[解读导读](../../../library/i-jepa.md) · [具身感知与场景表示](../../../paper-map/README.md#track-embodied-perception) · [CVPR集锦](../../../venues/CVPR/README.md)

[原文](https://openaccess.thecvf.com/content/CVPR2023/html/Assran_Self-Supervised_Learning_From_Images_With_a_Joint-Embedding_Predictive_Architecture_CVPR_2023_paper.html) · [PDF](https://openaccess.thecvf.com/content/CVPR2023/papers/Assran_Self-Supervised_Learning_From_Images_With_a_Joint-Embedding_Predictive_Architecture_CVPR_2023_paper.pdf) · [阅读卡片](../../../library/i-jepa.md)

## 机制简析

上下文编码器读取图像可见块，预测器根据目标位置预测多个缺失区域的表征，目标编码器生成需要拟合的监督向量。目标块足够大、上下文空间分布足够丰富，让任务偏向语义结构而非局部纹理补全。原文比较分类、目标计数、深度预测和掩码策略，后续时序 JEPA 再扩展预测对象。

带着这个问题读：世界模型必须把像素画出来吗，预测目标区域的 latent 会保留哪些可用信息？

初读判断：监督目标与掩码选择有可辨认机制，跨任务和设计消融扎实，官方代码公开；适合讲清具身世界模型里预测什么这一分歧。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 95.0 | 30% |
| 创新性 | 88 | 20% |
| 实验与证据 | 89 | 20% |
| 学术影响 | 75.2 | 10% |
| 近期关注 | 92.0 | 5% |
| 复用价值 | 92 | 8% |
| 阅读价值 | 96 | 7% |

刊会依据：[CVPR 2023](../../../venues/CVPR/README.md)，正式出处见[出版/原文记录](https://openaccess.thecvf.com/content/CVPR2023/html/Assran_Self-Supervised_Learning_From_Images_With_a_Joint-Embedding_Predictive_Architecture_CVPR_2023_paper.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：正式刊会版本；OpenAlex题目：Self-Supervised Learning from Images with a Joint-Embedding Predictive Architecture。累计被引 410，2025–2026 被引 304；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4386076428) · [文献计量条目](https://openalex.org/W4386076428)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
