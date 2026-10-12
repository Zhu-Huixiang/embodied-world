# SAM 星系

Segment Anything

**导读** · 具身感知与场景表示

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/sam.md) · [原文](https://openaccess.thecvf.com/content/ICCV2023/html/Kirillov_Segment_Anything_ICCV_2023_paper.html) · [评分卡](../../leaderboard/papers/sam/README.md)

图像编码器先算一次图像特征，点、框或已有掩码由提示编码器表达，轻量掩码解码器联合两者预测目标区域。一次图像编码可以服务多次交互，模型同时输出多个候选以应对提示歧义。数据引擎让模型辅助人工标注再改进模型，原文以零样本图像分割和不同提示任务验证迁移。

## 技术挂点

- [空间表示](../concepts/spatial.md)：保留像素、点、体素或对象相对位置的表示，让预测能接到几何与动作位置。

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。

- [零样本任务接口](../concepts/zero-shot.md)：不用目标数据集训练样本拟合分类头，而用任务描述等已有信息直接构造预测接口。

## 本篇行星与卫星

- [空间表示](sam/spatial.md) · 初读挂点
- [注意力](sam/attention.md) · 初读挂点
- [零样本任务接口](sam/zero-shot.md) · 初读挂点
- [本篇方法链路](sam/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
