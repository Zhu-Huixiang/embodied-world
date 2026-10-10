# Segment Anything

出处：ICCV 2023。研究范围：生成/表征基础，机器人目标区域、抓取候选与开放词汇感知的分割接口。

[原文入口](https://openaccess.thecvf.com/content/ICCV2023/html/Kirillov_Segment_Anything_ICCV_2023_paper.html) · [原文 PDF](https://openaccess.thecvf.com/content/ICCV2023/papers/Kirillov_Segment_Anything_ICCV_2023_paper.pdf) · [作者项目 / 代码入口](https://github.com/facebookresearch/segment-anything)

ICCV 2023 正式论文；收录提示分割基础，不将原文的图像分割评测解释为机器人控制结果。

阅读问题：**给视觉系统一个点或框，它怎样找到目标轮廓，哪些信息还需要控制策略来补？**

收录理由：提示分割把指定目标与像素区域接起来，是语言/视觉操作系统的重要感知接口；模型、训练数据和跨分布分割实验均公开。

证据入口：任务、模型和数据闭环连得清楚，大规模公开数据与跨域实验充足；读者能看懂分割接口怎样进入机器人感知链。

具身关联：提示分割把指定目标与像素区域接起来，是语言/视觉操作系统的重要感知接口；模型、训练数据和跨分布分割实验均公开。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/sam/README.md)

机制简析：图像编码器先算一次图像特征，点、框或已有掩码由提示编码器表达，轻量掩码解码器联合两者预测目标区域。一次图像编码可以服务多次交互，模型同时输出多个候选以应对提示歧义。数据引擎让模型辅助人工标注再改进模型，原文以零样本图像分割和不同提示任务验证迁移。
<!-- discovery:end -->
