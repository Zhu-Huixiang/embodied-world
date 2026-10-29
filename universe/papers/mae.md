# MAE 星系

Masked Autoencoders Are Scalable Vision Learners

**已精讲** · 具身感知与场景表示

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/mae-2111.06377/README.md) · [原文](https://openaccess.thecvf.com/content/CVPR2022/html/He_Masked_Autoencoders_Are_Scalable_Vision_Learners_CVPR_2022_paper.html) · [评分卡](../../leaderboard/papers/mae/README.md)

随机遮住大部分图像 patch，编码器只处理可见部分，轻量解码器再接入 mask token 还原缺失像素。非对称结构减少昂贵编码器的计算，高遮挡比例让补全任务需要理解物体和场景。原文比较分类、检测、分割迁移；MVP 将同类编码器冻结后接到可训练控制模块。

## 技术挂点

- [遮蔽预测](../concepts/masking.md)：隐藏部分输入，训练模型恢复像素、token 或表征。恢复什么决定监督重点。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/mae-2111.06377/README.md#31-a-区随机藏起来位置仍然留着)

- [视觉 patch token](../concepts/patches.md)：把图像切成块，展平并投影成向量，再加入位置信息。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/mae-2111.06377/README.md#31-a-区随机藏起来位置仍然留着)

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/mae-2111.06377/README.md#32-b-区昂贵的编码器只招待真有内容的客人)

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/mae-2111.06377/README.md#32-b-区昂贵的编码器只招待真有内容的客人)

- [线性探测](../concepts/linear-probe.md)：冻结编码器，用带标签的下游样本训练线性预测头，以检查特征本身是否容易迁移。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/mae-2111.06377/README.md#43-部分微调线性探测没看见的能力)

- [空间表示](../concepts/spatial.md)：保留像素、点、体素或对象相对位置的表示，让预测能接到几何与动作位置。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/mae-2111.06377/README.md#5-迁移实验离开分类考场之后)

## 本篇行星与卫星

- [遮蔽预测](mae/masking.md) · 已讲解
- [视觉 patch token](mae/patches.md) · 已讲解
- [表征空间](mae/representation.md) · 已讲解
- [注意力](mae/attention.md) · 已讲解
- [线性探测](mae/linear-probe.md) · 已讲解
- [空间表示](mae/spatial.md) · 已讲解
- [本篇方法链路](mae/method-chain.md) · 已讲解
- [随机高比例遮挡](mae/method-masking.md) · 已讲解
- [只编码可见块](mae/visible-encoder.md) · 已讲解
- [轻量重建解码器](mae/decoder.md) · 已讲解
- [遮挡像素目标](mae/pixel-target.md) · 已讲解
- [遮挡方式与比例](mae/mask-ablation.md) · 已讲解
- [实际计算节省](mae/wall-clock.md) · 已讲解
- [部分微调](mae/partial-finetune.md) · 已讲解
- [空间任务迁移](mae/spatial-transfer.md) · 已讲解

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
