# 视觉特征接入动作模型的实际路线 · DINOv2

OpenVLA用DINOv2与SigLIP分别编码图像，沿特征通道拼接后通过两层MLP接入语言模型。

最终VLA还用机器人动作数据训练并微调视觉编码器；这条后续系统链路说明视觉起点如何被使用，动作能力不由DINOv2单独产生。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#10-讨论从视觉特征走到机器人中间还缺什么)

[本篇星系](../dinov2.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md) · [原文依据](https://raw.githubusercontent.com/mlresearch/v270/main/assets/kim25c/kim25c.pdf)
