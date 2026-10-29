# 视觉 patch token · DINO

把图像切成块，展平并投影成向量，再加入位置信息。

CLIP B/32 的 224×224 图像得到 49 个图块，加 CLS 共 50 个视觉位置。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dino-2104.14294/README.md#52-图块变小参数没涨账单照涨)

[跨论文技术入口](../../concepts/patches.md)

[本篇星系](../dino.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dino-2104.14294/README.md) · [原文依据](https://openaccess.thecvf.com/content/ICCV2021/html/Caron_Emerging_Properties_in_Self-Supervised_Vision_Transformers_ICCV_2021_paper.html)
