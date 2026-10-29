# DINO 星系

Emerging Properties in Self-Supervised Vision Transformers

**已精讲** · 具身感知与场景表示

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dino-2104.14294/README.md) · [原文](https://openaccess.thecvf.com/content/ICCV2021/html/Caron_Emerging_Properties_in_Self-Supervised_Vision_Transformers_ICCV_2021_paper.html) · [评分卡](../../leaderboard/papers/dino/README.md)

同一图像的不同裁剪分别进入学生和教师，学生用交叉熵拟合教师输出的概率分布。教师参数由学生参数的指数滑动平均更新，中心化与温度锐化防止两者退化成常量。原文比较 ViT 与卷积网络，检查 k-NN、线性分类和注意力中出现的物体区域结构。

## 技术挂点

- [教师学生蒸馏](../concepts/distill.md)：用教师的预测或动作监督学生，让部署模型复制可用行为。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dino-2104.14294/README.md#34-d-区老师慢一点训练才有个相对稳的目标)

- [交叉熵](../concepts/cross-entropy.md)：正确候选的负对数概率。正确项概率越小，损失越大，梯度会推动正确分数上升。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dino-2104.14294/README.md#33-c-区把分数变分布再跨视图对答案)

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dino-2104.14294/README.md#32-b-区骨干负责看投影头负责训练对齐)

- [softmax 与温度](../concepts/softmax.md)：对候选分数取指数后归一化为总和为 1 的概率。温度控制分差如何影响概率。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dino-2104.14294/README.md#33-c-区把分数变分布再跨视图对答案)

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dino-2104.14294/README.md#42-表示的新性质从找同类到找物体)

- [视觉 patch token](../concepts/patches.md)：把图像切成块，展平并投影成向量，再加入位置信息。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dino-2104.14294/README.md#52-图块变小参数没涨账单照涨)

- [空间表示](../concepts/spatial.md)：保留像素、点、体素或对象相对位置的表示，让预测能接到几何与动作位置。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dino-2104.14294/README.md#42-表示的新性质从找同类到找物体)

- [线性探测](../concepts/linear-probe.md)：冻结编码器，用带标签的下游样本训练线性预测头，以检查特征本身是否容易迁移。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dino-2104.14294/README.md#41-最普通的分类读出方式却要分清)

## 本篇行星与卫星

- [教师学生蒸馏](dino/distill.md) · 已讲解
- [交叉熵](dino/cross-entropy.md) · 已讲解
- [表征空间](dino/representation.md) · 已讲解
- [softmax 与温度](dino/softmax.md) · 已讲解
- [注意力](dino/attention.md) · 已讲解
- [视觉 patch token](dino/patches.md) · 已讲解
- [空间表示](dino/spatial.md) · 已讲解
- [线性探测](dino/linear-probe.md) · 已讲解
- [本篇方法链路](dino/method-chain.md) · 已讲解
- [局部对齐整体](dino/multicrop.md) · 已讲解
- [训练投影头](dino/projection.md) · 已讲解
- [温度软分布](dino/soft-target.md) · 已讲解
- [跨视图交叉熵](dino/cross-view.md) · 已讲解
- [动量教师](dino/teacher-ema.md) · 已讲解
- [输出中心统计](dino/center.md) · 已讲解
- [防止表示坍塌](dino/collapse.md) · 已讲解
- [加权近邻读出](dino/knn.md) · 已讲解
- [注意力区域与阈值](dino/attention-mask.md) · 已讲解
- [冻结特征跨帧对应](dino/patch-correspondence.md) · 已讲解
- [小图块的计算代价](dino/patch-cost.md) · 已讲解

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
