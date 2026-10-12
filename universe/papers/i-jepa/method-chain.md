# 本篇方法链路 · I-JEPA

上下文编码器读取图像可见块，预测器根据目标位置预测多个缺失区域的表征，目标编码器生成需要拟合的监督向量。目标块足够大、上下文空间分布足够丰富，让任务偏向语义结构而非局部纹理补全。原文比较分类、目标计数、深度预测和掩码策略，后续时序 JEPA 再扩展预测对象。

上下文编码器读取图像可见块，预测器根据目标位置预测多个缺失区域的表征，目标编码器生成需要拟合的监督向量。目标块足够大、上下文空间分布足够丰富，让任务偏向语义结构而非局部纹理补全。原文比较分类、目标计数、深度预测和掩码策略，后续时序 JEPA 再扩展预测对象。

[本篇星系](../i-jepa.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/i-jepa.md) · [原文依据](https://openaccess.thecvf.com/content/CVPR2023/html/Assran_Self-Supervised_Learning_From_Images_With_a_Joint-Embedding_Predictive_Architecture_CVPR_2023_paper.html)
