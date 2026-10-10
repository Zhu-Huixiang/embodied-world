# Segment Anything

**解读导读** · ICCV 2023 · [具身感知与场景表示](../paper-map/README.md#track-embodied-perception)

研究范围：生成/表征基础，机器人目标区域、抓取候选与开放词汇感知的分割接口。

[原文入口](https://openaccess.thecvf.com/content/ICCV2023/html/Kirillov_Segment_Anything_ICCV_2023_paper.html) · [原文 PDF](https://openaccess.thecvf.com/content/ICCV2023/papers/Kirillov_Segment_Anything_ICCV_2023_paper.pdf) · [作者项目 / 代码入口](https://github.com/facebookresearch/segment-anything) · [作者与团队](../leaderboard/origins/papers/sam.md)

ICCV 2023 正式论文；收录提示分割基础，不将原文的图像分割评测解释为机器人控制结果。

## 先看它做了什么

图像编码器先算一次图像特征，点、框或已有掩码由提示编码器表达，轻量掩码解码器联合两者预测目标区域。一次图像编码可以服务多次交互，模型同时输出多个候选以应对提示歧义。数据引擎让模型辅助人工标注再改进模型，原文以零样本图像分割和不同提示任务验证迁移。

## 带着什么问题读

**给视觉系统一个点或框，它怎样找到目标轮廓，哪些信息还需要控制策略来补？**

## 为什么值得继续读

提示分割把指定目标与像素区域接起来，是语言/视觉操作系统的重要感知接口；模型、训练数据和跨分布分割实验均公开。

证据入口：任务、模型和数据闭环连得清楚，大规模公开数据与跨域实验充足；读者能看懂分割接口怎样进入机器人感知链。

具身关联：提示分割把指定目标与像素区域接起来，是语言/视觉操作系统的重要感知接口；模型、训练数据和跨分布分割实验均公开。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/sam/README.md) · [ICCV集锦](../venues/ICCV/README.md) · [地图方向](../paper-map/README.md#track-embodied-perception) · [首页](../README.md)

元数据核对：2026-10-10。
