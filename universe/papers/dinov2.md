# DINOv2 星系

DINOv2: Learning Robust Visual Features without Supervision

**已精讲** · 具身感知与场景表示

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md) · [原文](https://openreview.net/forum?id=a68SUt6zFt) · [评分卡](../../leaderboard/papers/dinov2/README.md)

在大规模筛选图像上扩展图像级与 patch 级自监督学习，再把大 ViT 教师蒸馏为不同尺寸的编码器。下游可以冻结 backbone，用轻量预测头读取分类、分割或深度相关信息。原文比较多种图像与像素任务；OpenVLA 的视觉输入实际将 DINOv2 特征与 SigLIP 特征拼接后映射给语言模型。

## 技术挂点

- [教师学生蒸馏](../concepts/distill.md)：用教师的预测分布、特征或动作监督学生，把已有模型的可用信息迁移到学生。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#52-蒸馏时教师的更新规则变了)

- [视觉 patch token](../concepts/patches.md)：把图像切成块，展平并投影成向量，再加入位置信息。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#41-图像怎样变成-token)

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#1-引言一套特征能不能少为每个任务重练一次)

- [向量归一化](../concepts/normalization.md)：把向量除以自己的 L2 长度，得到单位向量。点积随后比较方向，减少向量大小的干扰。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#45-koleo-与高分辨率让特征分得开也看得细)

- [余弦相似度](../concepts/cosine.md)：两个向量点积再除以各自长度。单位向量的点积直接等于余弦相似度。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#3-数据处理样本变多之前先看覆盖有没有变)

- [交叉熵](../concepts/cross-entropy.md)：用目标概率分布加权预测概率的负对数，再求和。目标集中在一个正确类别时，就是该类别的负对数概率。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#42-dino不同裁剪对齐整图判断)

- [softmax 与温度](../concepts/softmax.md)：对候选分数取指数后归一化为总和为 1 的概率。温度控制分差如何影响概率。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#7-结果冻结特征不等于免训练)

- [线性探测](../concepts/linear-probe.md)：冻结编码器，用带标签的下游样本训练线性预测头，以检查特征本身是否容易迁移。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#71-imagenet-与分布变化)

- [分布偏移](../concepts/shift.md)：测试场景的画风、视角、背景或对象组合发生变化，模型习惯的视觉线索随之改变。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#71-imagenet-与分布变化)

- [Transformer](../concepts/transformer.md)：用注意力交换 token 信息，再逐位置加工。token 可以来自字词、图像块、状态或动作。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#41-图像怎样变成-token)

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#51-计算工程怎样改变可训练规模)

- [遮蔽预测](../concepts/masking.md)：隐藏部分输入，训练模型恢复像素、token 或表征。恢复什么决定监督重点。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#43-ibot遮住局部对齐对应位置)

- [泛化评测与遗忘](../concepts/benchmark.md)：拆开任务、物体、场景或学习顺序，检查迁移能力和旧技能保留。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/dinov2-2304.07193/README.md#71-imagenet-与分布变化)

## 本篇行星与卫星

- [教师学生蒸馏](dinov2/distill.md) · 已讲解
- [视觉 patch token](dinov2/patches.md) · 已讲解
- [表征空间](dinov2/representation.md) · 已讲解
- [向量归一化](dinov2/normalization.md) · 已讲解
- [余弦相似度](dinov2/cosine.md) · 已讲解
- [交叉熵](dinov2/cross-entropy.md) · 已讲解
- [softmax 与温度](dinov2/softmax.md) · 已讲解
- [线性探测](dinov2/linear-probe.md) · 已讲解
- [分布偏移](dinov2/shift.md) · 已讲解
- [Transformer](dinov2/transformer.md) · 已讲解
- [注意力](dinov2/attention.md) · 已讲解
- [遮蔽预测](dinov2/masking.md) · 已讲解
- [泛化评测与遗忘](dinov2/benchmark.md) · 已讲解
- [本篇方法链路](dinov2/method-chain.md) · 已讲解
- [冻结视觉骨干的目标](dinov2/frozen-features.md) · 已讲解
- [配文与像素信息的取舍](dinov2/caption-detail.md) · 已讲解
- [靠视觉检索整理训练集](dinov2/curated-retrieval.md) · 已讲解
- [先去重再扩展覆盖](dinov2/deduplication.md) · 已讲解
- [大图像域逐样本取近邻](dinov2/sample-retrieval.md) · 已讲解
- [小数据域按簇扩充并封顶](dinov2/cluster-retrieval.md) · 已讲解
- [预训练、检索种子与评测分开](dinov2/dataset-roles.md) · 已讲解
- [一个整图token和一组局部token](dinov2/patch-cls.md) · 已讲解
- [跨裁切匹配整图分布](dinov2/dino-image-loss.md) · 已讲解
- [遮挡图块预测teacher特征](dinov2/ibot-patch-loss.md) · 已讲解
- [图像头和图块头分开](dinov2/untied-heads.md) · 已讲解
- [参数平均产生缓慢teacher](dinov2/ema-teacher.md) · 已讲解
- [批内原型分配的归一化](dinov2/sinkhorn.md) · 已讲解
- [让同批特征保持展开](dinov2/koleo.md) · 已讲解
- [末段提高图像分辨率](dinov2/high-res-tail.md) · 已讲解
- [打包序列却隔开注意力](dinov2/packed-attention.md) · 已讲解
- [被丢弃分支不再白算](dinov2/stochastic-depth.md) · 已讲解
- [分片训练状态](dinov2/fsdp.md) · 已讲解
- [用冻结巨型teacher训练小模型](dinov2/fixed-teacher-distill.md) · 已讲解
- [配方改善不等于每项指标都涨](dinov2/recipe-ablation.md) · 已讲解
- [同规模随机数据仍可能差一截](dinov2/data-ablation.md) · 已讲解
- [模型变大后更需要数据覆盖](dinov2/scale-interaction.md) · 已讲解
- [分开检验全局展开与局部监督](dinov2/loss-ablation.md) · 已讲解
- [蒸馏优势看同结构对照](dinov2/distill-evidence.md) · 已讲解
- [用短尾阶段换取高分辨率收益](dinov2/resolution-evidence.md) · 已讲解
- [冻结骨干仍要训练读出](dinov2/linear-protocol.md) · 已讲解
- [整套系统对照与单模块归因分开](dinov2/classifier-comparison.md) · 已讲解
- [域偏移收益并不均匀](dinov2/robustness-scope.md) · 已讲解
- [把图像特征汇成视频读出](dinov2/frame-video.md) · 已讲解
- [用特征相似度找同一对象](dinov2/instance-ranking.md) · 已讲解
- [从局部token读出像素类别](dinov2/segmentation-readout.md) · 已讲解
- [冻结骨干外面仍可接复杂解码器](dinov2/adapter-readout.md) · 已讲解
- [有监督深度头把特征转成距离](dinov2/depth-readout.md) · 已讲解
- [主成分颜色展示部件关联](dinov2/pca-parts.md) · 已讲解
- [局部匹配需要距离分配与筛选](dinov2/patch-assignment.md) · 已讲解
- [无标签训练仍可能有地域偏差](dinov2/fairness-gap.md) · 已讲解
- [有害标签测试有指定集合和阈值](dinov2/association-test.md) · 已讲解
- [单次复训与整个研究成本分开](dinov2/carbon-account.md) · 已讲解
- [视觉表示到机器人行动之间还有接口](dinov2/robotics-boundary.md) · 已讲解
- [视觉特征接入动作模型的实际路线](dinov2/openvla-interface.md) · 已讲解

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
