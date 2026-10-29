# 本篇方法链路 · JAM

JAM把骨干初始化、未来监督和部署模块拆开：当前图像/语言经骨干提供视觉token，动作专家结合状态生成动作块。训练时，记录的未来只送入冻结anchor得到目标；一个额外prediction head从当前特征预测这些目标，以逐token/时间偏移的余弦距离加动作flow-matching损失训练，目标停止梯度。部署删除anchor和prediction head，动作路径不读未来，也不生成未来图像。固定未来目标可提前缓存；Wan配置以VAE直接编码目标最好，Ovis配置则用Yak特征，不能把结论简化成越大的未来模型越好。

JAM把骨干初始化、未来监督和部署模块拆开：当前图像/语言经骨干提供视觉token，动作专家结合状态生成动作块。训练时，记录的未来只送入冻结anchor得到目标；一个额外prediction head从当前特征预测这些目标，以逐token/时间偏移的余弦距离加动作flow-matching损失训练，目标停止梯度。部署删除anchor和prediction head，动作路径不读未来，也不生成未来图像。固定未来目标可提前缓存；Wan配置以VAE直接编码目标最好，Ovis配置则用Yak特征，不能把结论简化成越大的未来模型越好。

[本篇星系](../jam.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/jam.md) · [原文依据](https://arxiv.org/abs/2610.37219v1)
