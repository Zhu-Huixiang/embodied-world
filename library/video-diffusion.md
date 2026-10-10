# Video Diffusion Models

**解读导读** · NeurIPS 2022 · [视频与序列生成](../paper-map/README.md#track-video-generation)

研究范围：生成/表征基础，视频世界模型与视频动作模型的时空去噪结构。

[原文入口](https://proceedings.neurips.cc/paper_files/paper/2022/hash/39235c56aef13fb05a6adc95eb9d8d66-Abstract-Conference.html) · [原文 PDF](https://proceedings.neurips.cc/paper_files/paper/2022/file/39235c56aef13fb05a6adc95eb9d8d66-Paper-Conference.pdf) · [作者项目 / 代码入口](https://video-diffusion.github.io/)

NeurIPS 2022 正式论文；只记录原始视频生成/预测评测，动作条件和机器人闭环需读下游方法。

## 先看它做了什么

把图像扩散 U-Net 扩成空间与时间分解的网络，空间卷积处理每帧内容，时间注意力在对应位置之间传信息。图像与视频联合训练共享视觉能力，再以条件采样扩展时间和空间范围。原文在视频预测、无条件视频与文本条件视频任务比较生成质量和时序一致性。

## 带着什么问题读

**逐帧画图为什么会抖，空间与时间注意力怎样让一段未来视频连起来？**

## 为什么值得继续读

将图像去噪扩展到时空序列、联合使用图像和视频数据、做条件续帧，是后续视频世界生成的直接基础问题。

证据入口：时空结构和联合训练的设计明确，跨生成任务有原始对照；作者演示公开，复用分低于完整开放训练权重的基础项目。

具身关联：将图像去噪扩展到时空序列、联合使用图像和视频数据、做条件续帧，是后续视频世界生成的直接基础问题。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/video-diffusion/README.md) · [NeurIPS集锦](../venues/NeurIPS/README.md) · [地图方向](../paper-map/README.md#track-video-generation) · [首页](../README.md)

元数据核对：2026-10-10。
