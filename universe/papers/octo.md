# Octo 星系

Octo: An Open-Source Generalist Robot Policy

**导读** · 视觉语言动作模型 VLA

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/octo.md) · [原文](https://www.roboticsproceedings.org/rss20/p090.html) · [评分卡](../../leaderboard/papers/octo/README.md)

各类任务、图像和本体感觉先由模态 tokenizer 转成 token，Transformer 主干处理后由读取头和扩散解码器产生动作块。更换机器人时，输入或输出适配器可改变，而主干保留预训练知识并微调。项目在不同平台上区分零样本运行与小数据微调，还单独检验新力传感输入和关节控制空间。

## 技术挂点

- [扩散去噪](../concepts/diffusion.md)：训练网络从带噪对象估计噪声或干净目标，生成时从噪声开始迭代恢复样本。

- [动作块](../concepts/chunk.md)：一次预测多个未来控制时刻的动作，再执行部分并用新观测更新。

- [跨本体数据](../concepts/cross-body.md)：从多个机器人或人类收集经验，通过动作/观测适配接到共享学习系统。

## 本篇行星与卫星

- [扩散去噪](octo/diffusion.md) · 初读挂点
- [动作块](octo/chunk.md) · 初读挂点
- [跨本体数据](octo/cross-body.md) · 初读挂点
- [本篇方法链路](octo/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
