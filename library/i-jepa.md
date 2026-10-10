# Self-Supervised Learning from Images with a Joint-Embedding Predictive Architecture

出处：CVPR 2023。研究范围：生成/表征基础，具身潜表征预测与 JEPA 世界模型的图像起点。

[原文入口](https://openaccess.thecvf.com/content/CVPR2023/html/Assran_Self-Supervised_Learning_From_Images_With_a_Joint-Embedding_Predictive_Architecture_CVPR_2023_paper.html) · [原文 PDF](https://openaccess.thecvf.com/content/CVPR2023/papers/Assran_Self-Supervised_Learning_From_Images_With_a_Joint-Embedding_Predictive_Architecture_CVPR_2023_paper.pdf) · [作者项目 / 代码入口](https://github.com/facebookresearch/ijepa)

CVPR 2023 正式论文；I-JEPA 是同一图像内的表征预测，不将其写成已经学习动作条件动力学或机器人控制。

阅读问题：**世界模型必须把像素画出来吗，预测目标区域的 latent 会保留哪些可用信息？**

收录理由：在表示空间预测而非重建像素，是后续 JEPA 型世界模型的重要机制基础；和 MAE 并读能解释为何监督对象不同会影响任务信息。

证据入口：监督目标与掩码选择有可辨认机制，跨任务和设计消融扎实，官方代码公开；适合讲清具身世界模型里预测什么这一分歧。

具身关联：在表示空间预测而非重建像素，是后续 JEPA 型世界模型的重要机制基础；和 MAE 并读能解释为何监督对象不同会影响任务信息。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/i-jepa/README.md)

机制简析：上下文编码器读取图像可见块，预测器根据目标位置预测多个缺失区域的表征，目标编码器生成需要拟合的监督向量。目标块足够大、上下文空间分布足够丰富，让任务偏向语义结构而非局部纹理补全。原文比较分类、目标计数、深度预测和掩码策略，后续时序 JEPA 再扩展预测对象。
<!-- discovery:end -->
