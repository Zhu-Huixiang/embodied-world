# Video Diffusion 星系

Video Diffusion Models

**导读** · 视频与序列生成

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/video-diffusion.md) · [原文](https://proceedings.neurips.cc/paper_files/paper/2022/hash/39235c56aef13fb05a6adc95eb9d8d66-Abstract-Conference.html) · [评分卡](../../leaderboard/papers/video-diffusion/README.md)

把图像扩散 U-Net 扩成空间与时间分解的网络，空间卷积处理每帧内容，时间注意力在对应位置之间传信息。图像与视频联合训练共享视觉能力，再以条件采样扩展时间和空间范围。原文在视频预测、无条件视频与文本条件视频任务比较生成质量和时序一致性。

## 技术挂点

- [视频时序生成](../concepts/video.md)：同时表达画面内容与时间变化，用历史与条件产生连续帧。

- [扩散去噪](../concepts/diffusion.md)：训练网络从带噪对象估计噪声或干净目标，生成时从噪声开始迭代恢复样本。

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。

## 本篇行星与卫星

- [视频时序生成](video-diffusion/video.md) · 初读挂点
- [扩散去噪](video-diffusion/diffusion.md) · 初读挂点
- [注意力](video-diffusion/attention.md) · 初读挂点
- [本篇方法链路](video-diffusion/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
