# 本篇方法链路 · Video Diffusion

把图像扩散 U-Net 扩成空间与时间分解的网络，空间卷积处理每帧内容，时间注意力在对应位置之间传信息。图像与视频联合训练共享视觉能力，再以条件采样扩展时间和空间范围。原文在视频预测、无条件视频与文本条件视频任务比较生成质量和时序一致性。

把图像扩散 U-Net 扩成空间与时间分解的网络，空间卷积处理每帧内容，时间注意力在对应位置之间传信息。图像与视频联合训练共享视觉能力，再以条件采样扩展时间和空间范围。原文在视频预测、无条件视频与文本条件视频任务比较生成质量和时序一致性。

[本篇星系](../video-diffusion.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/video-diffusion.md) · [原文依据](https://proceedings.neurips.cc/paper_files/paper/2022/hash/39235c56aef13fb05a6adc95eb9d8d66-Abstract-Conference.html)
