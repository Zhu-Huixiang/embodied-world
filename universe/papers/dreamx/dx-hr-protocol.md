# 1008段视频如何做零样本迁移评估 · DreamX

H&R共21任务，每任务48clip，使用人类源片段和对应机器人的首帧。

不以配对数据训练；输出统一取前20帧并去掉条件帧，19帧用于FVD/LPIPS/PSNR/SSIM。指标衡量生成视频，不是1008次真机试验。

继续拆：[视频迁移保运动也保目标外观](dx-hr-results.md)。

[本篇星系](../dreamx.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamx.md) · [原文依据](https://arxiv.org/pdf/2611.05377v1)
