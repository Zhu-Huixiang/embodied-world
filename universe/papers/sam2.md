# SAM 2 星系

SAM 2: Segment Anything in Images and Videos

**已精讲** · 具身感知与场景表示

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam2-2408.00714/README.md) · [原文](https://openreview.net/forum?id=Ha6RTeWMd0) · [评分卡](../../leaderboard/papers/sam2/README.md)

逐帧图像特征通过记忆注意力读取之前的目标提示与掩码信息，再与当前提示一起预测本帧掩码。记忆编码器把当前预测存入记忆，下一帧继续使用；静态图像相当于记忆为空的视频。原文比较交互次数、速度以及图像和视频分割基准。

## 技术挂点

- [空间表示](../concepts/spatial.md)：保留像素、点、体素或对象相对位置的表示，让预测能接到几何与动作位置。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam2-2408.00714/README.md#41-a-区一张图先变成多尺度特征)

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam2-2408.00714/README.md#42-b-区记忆里放的不是整段录像)

- [闭环滚动与历史偏移](../concepts/rollout.md)：重复预测、执行或生成，把新观测或模型历史接回后续计算。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam2-2408.00714/README.md#44-d-区把这次预测写进下次的条件)

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam2-2408.00714/README.md#41-a-区一张图先变成多尺度特征)

- [Transformer](../concepts/transformer.md)：用注意力交换 token 信息，再逐位置加工。token 可以来自字词、图像块、状态或动作。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam2-2408.00714/README.md#43-c-区点击候选掩码与它现在不在)

- [交叉熵](../concepts/cross-entropy.md)：正确候选的负对数概率。正确项概率越小，损失越大，梯度会推动正确分数上升。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam2-2408.00714/README.md#45-e-区训练时怎样教它别跟丢)

- [零样本任务接口](../concepts/zero-shot.md)：不用目标数据集训练样本拟合分类头，而用任务描述等已有信息直接构造预测接口。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam2-2408.00714/README.md#61-先认指标再看交互曲线)

- [泛化评测与遗忘](../concepts/benchmark.md)：拆开任务、物体、场景或学习顺序，检查迁移能力和旧技能保留。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam2-2408.00714/README.md#62-只在第一帧给提示还能传多远)

- [分布偏移](../concepts/shift.md)：测试场景的画风、视角、背景或对象组合发生变化，模型习惯的视觉线索随之改变。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam2-2408.00714/README.md#8-结论它给机器人补了哪块感知拼图)

## 本篇行星与卫星

- [空间表示](sam2/spatial.md) · 已讲解
- [注意力](sam2/attention.md) · 已讲解
- [闭环滚动与历史偏移](sam2/rollout.md) · 已讲解
- [表征空间](sam2/representation.md) · 已讲解
- [Transformer](sam2/transformer.md) · 已讲解
- [交叉熵](sam2/cross-entropy.md) · 已讲解
- [零样本任务接口](sam2/zero-shot.md) · 已讲解
- [泛化评测与遗忘](sam2/benchmark.md) · 已讲解
- [分布偏移](sam2/shift.md) · 已讲解
- [本篇方法链路](sam2/method-chain.md) · 已讲解
- [可提示视频分割](sam2/sam2-pvs.md) · 已讲解
- [层次特征与细节旁路](sam2/sam2-hiera.md) · 已讲解
- [空间记忆与提示队列](sam2/sam2-bank.md) · 已讲解
- [对象指针](sam2/sam2-ptr.md) · 已讲解
- [跨帧记忆读取](sam2/sam2-read.md) · 已讲解
- [双向掩码解码](sam2/sam2-decoder.md) · 已讲解
- [多候选与质量预测](sam2/sam2-ambiguity.md) · 已讲解
- [对象缺席判断](sam2/sam2-presence.md) · 已讲解
- [对象记忆写入](sam2/sam2-write.md) · 已讲解
- [多对象计算分工](sam2/sam2-multiobject.md) · 已讲解
- [掩码与存在性联合监督](sam2/sam2-loss.md) · 已讲解
- [十六帧难例微调](sam2/sam2-longtrain.md) · 已讲解
- [人机标注循环](sam2/sam2-engine.md) · 已讲解
- [区域边界与交互预算](sam2/sam2-metric.md) · 已讲解
- [图像与视频两把秒表](sam2/sam2-speed.md) · 已讲解
- [记忆容量取舍](sam2/sam2-memtradeoff.md) · 已讲解

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
