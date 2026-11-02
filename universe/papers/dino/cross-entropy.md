# 交叉熵 · DINO

用目标概率分布加权预测概率的负对数，再求和。目标集中在一个正确类别时，就是该类别的负对数概率。

CLIP用配对图文的位置作目标；DINOv2用教师给出的软分布监督学生。目标分布自身有熵，预测对齐后交叉熵也未必为零。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dino-2104.14294/README.md#33-c-区把分数变分布再跨视图对答案)

继续拆：[softmax 与温度](softmax.md)。

[跨论文技术入口](../../concepts/cross-entropy.md)

[本篇星系](../dino.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dino-2104.14294/README.md) · [原文依据](https://openaccess.thecvf.com/content/ICCV2021/html/Caron_Emerging_Properties_in_Self-Supervised_Vision_Transformers_ICCV_2021_paper.html)
