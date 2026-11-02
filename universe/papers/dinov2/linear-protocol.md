# 冻结骨干仍要训练读出 · DINOv2

ImageNet线性评估使用标签优化分类头，搜索学习率、层数和patch汇总方式。

Appendix B.3会选择学习率、输出层数和是否拼接平均patch特征，再报告验证集最优结果；冻结骨干不等于头部没有调参。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#71-imagenet-与分布变化)

继续拆：[整套系统对照与单模块归因分开](classifier-comparison.md) · [域偏移收益并不均匀](robustness-scope.md)。

[本篇星系](../dinov2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md) · [原文依据](https://arxiv.org/pdf/2304.07193v2)
