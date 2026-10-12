# MAE 星系

Masked Autoencoders Are Scalable Vision Learners

**导读** · 具身感知与场景表示

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/mae.md) · [原文](https://openaccess.thecvf.com/content/CVPR2022/html/He_Masked_Autoencoders_Are_Scalable_Vision_Learners_CVPR_2022_paper.html) · [评分卡](../../leaderboard/papers/mae/README.md)

随机遮住大部分图像 patch，编码器只处理可见部分，轻量解码器再接入 mask token 还原缺失像素。非对称结构减少昂贵编码器的计算，高遮挡比例让补全任务需要理解物体和场景。原文比较分类、检测、分割迁移；MVP 将同类编码器冻结后接到可训练控制模块。

## 技术挂点

- [遮蔽预测](../concepts/masking.md)：隐藏部分输入，训练模型恢复像素、token 或表征。恢复什么决定监督重点。

- [视觉 patch token](../concepts/patches.md)：把图像切成块，展平并投影成向量，再加入位置信息。

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。

## 本篇行星与卫星

- [遮蔽预测](mae/masking.md) · 初读挂点
- [视觉 patch token](mae/patches.md) · 初读挂点
- [表征空间](mae/representation.md) · 初读挂点
- [本篇方法链路](mae/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
