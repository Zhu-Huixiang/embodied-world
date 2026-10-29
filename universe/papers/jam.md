# JAM 星系

Vision-Language-Action or World-Action? Just Action Models

**导读** · 视觉语言动作模型 VLA

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/jam.md) · [原文](https://arxiv.org/abs/2610.37219v1) · [评分卡](../../leaderboard/papers/jam/README.md)

JAM把骨干初始化、未来监督和部署模块拆开：当前图像/语言经骨干提供视觉token，动作专家结合状态生成动作块。训练时，记录的未来只送入冻结anchor得到目标；一个额外prediction head从当前特征预测这些目标，以逐token/时间偏移的余弦距离加动作flow-matching损失训练，目标停止梯度。部署删除anchor和prediction head，动作路径不读未来，也不生成未来图像。固定未来目标可提前缓存；Wan配置以VAE直接编码目标最好，Ovis配置则用Yak特征，不能把结论简化成越大的未来模型越好。

## 技术挂点

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。

- [表征预测 JEPA](../concepts/jepa.md)：在表征空间预测目标而不是逐像素重建；防止表征坍缩仍需要相应设计。

- [余弦相似度](../concepts/cosine.md)：两个向量点积再除以各自长度。单位向量的点积直接等于余弦相似度。

- [Flow Matching](../concepts/flow.md)：给噪声到数据指定概率路径，回归沿路径的速度场；生成时数值积分这个场。

- [动作块](../concepts/chunk.md)：一次预测多个未来控制时刻的动作，再执行部分并用新观测更新。

- [变分自编码器 VAE](../concepts/vae.md)：编码器描述潜变量分布，解码器从潜变量重建样本，用重建与分布正则共同训练。

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。

- [分布偏移](../concepts/shift.md)：测试场景的画风、视角、背景或对象组合发生变化，模型习惯的视觉线索随之改变。

- [泛化评测与遗忘](../concepts/benchmark.md)：拆开任务、物体、场景或学习顺序，检查迁移能力和旧技能保留。

## 本篇行星与卫星

- [表征空间](jam/representation.md) · 初读挂点
- [表征预测 JEPA](jam/jepa.md) · 初读挂点
- [余弦相似度](jam/cosine.md) · 初读挂点
- [Flow Matching](jam/flow.md) · 初读挂点
- [动作块](jam/chunk.md) · 初读挂点
- [变分自编码器 VAE](jam/vae.md) · 初读挂点
- [动作表示](jam/action.md) · 初读挂点
- [分布偏移](jam/shift.md) · 初读挂点
- [泛化评测与遗忘](jam/benchmark.md) · 初读挂点
- [本篇方法链路](jam/method-chain.md) · 初读挂点
- [骨干、目标与部署的三项选择](jam/choices.md) · 初读挂点
- [当前观测到动作上下文](jam/current.md) · 初读挂点
- [冻结未来目标分支](jam/anchor.md) · 初读挂点
- [当前token预测未来特征](jam/head.md) · 初读挂点
- [动作损失与预见损失](jam/loss.md) · 初读挂点
- [删除训练期分支](jam/deploy.md) · 初读挂点
- [未来目标取什么表征](jam/targets.md) · 初读挂点
- [匹配子集上的扰动评估](jam/robustness.md) · 初读挂点
- [缓存后的在线训练成本](jam/cost.md) · 初读挂点
- [任务bootstrap与重复训练](jam/uncertainty.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
