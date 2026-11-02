# 把图像特征汇成视频读出 · DINOv2

视频评测取8个均匀帧，UCF/K400平均特征，SSv2拼接特征。

冻结图像骨干并训练线性头；这里没有动作条件预测或视频生成，SSv2的iBOT38.7仍高于DINOv2-g38.3。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#72-其他图像与视频分类)

[本篇星系](../dinov2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md) · [原文依据](https://arxiv.org/pdf/2304.07193v2)
