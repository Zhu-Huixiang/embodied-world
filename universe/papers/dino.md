# DINO 星系

Emerging Properties in Self-Supervised Vision Transformers

**导读** · 具身感知与场景表示

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dino.md) · [原文](https://openaccess.thecvf.com/content/ICCV2021/html/Caron_Emerging_Properties_in_Self-Supervised_Vision_Transformers_ICCV_2021_paper.html) · [评分卡](../../leaderboard/papers/dino/README.md)

同一图像的不同裁剪分别进入学生和教师，学生用交叉熵拟合教师输出的概率分布。教师参数由学生参数的指数滑动平均更新，中心化与温度锐化防止两者退化成常量。原文比较 ViT 与卷积网络，检查 k-NN、线性分类和注意力中出现的物体区域结构。

## 技术挂点

- [教师学生蒸馏](../concepts/distill.md)：用教师的预测或动作监督学生，让部署模型复制可用行为。

- [交叉熵](../concepts/cross-entropy.md)：正确候选的负对数概率。正确项概率越小，损失越大，梯度会推动正确分数上升。

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。

## 本篇行星与卫星

- [教师学生蒸馏](dino/distill.md) · 初读挂点
- [交叉熵](dino/cross-entropy.md) · 初读挂点
- [表征空间](dino/representation.md) · 初读挂点
- [本篇方法链路](dino/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
