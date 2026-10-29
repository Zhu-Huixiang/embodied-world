# 视觉 patch token · MAE

把图像切成块，展平并投影成向量，再加入位置信息。

CLIP B/32 的 224×224 图像得到 49 个图块，加 CLS 共 50 个视觉位置。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/mae-2111.06377/README.md#31-a-区随机藏起来位置仍然留着)

[跨论文技术入口](../../concepts/patches.md)

[本篇星系](../mae.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/mae-2111.06377/README.md) · [原文依据](https://openaccess.thecvf.com/content/CVPR2022/html/He_Masked_Autoencoders_Are_Scalable_Vision_Learners_CVPR_2022_paper.html)
