# 本篇方法链路 · SAM

图像编码器先算一次图像特征，点、框或已有掩码由提示编码器表达，轻量掩码解码器联合两者预测目标区域。一次图像编码可以服务多次交互，模型同时输出多个候选以应对提示歧义。数据引擎让模型辅助人工标注再改进模型，原文以零样本图像分割和不同提示任务验证迁移。

图像编码器先算一次图像特征，点、框或已有掩码由提示编码器表达，轻量掩码解码器联合两者预测目标区域。一次图像编码可以服务多次交互，模型同时输出多个候选以应对提示歧义。数据引擎让模型辅助人工标注再改进模型，原文以零样本图像分割和不同提示任务验证迁移。

[本篇星系](../sam.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam-2304.02643/README.md) · [原文依据](https://openaccess.thecvf.com/content/ICCV2023/html/Kirillov_Segment_Anything_ICCV_2023_paper.html)
