# DDPM 星系

Denoising Diffusion Probabilistic Models

**已精讲** · Diffusion / Transformer 基础

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md) · [原文](https://proceedings.neurips.cc/paper/2020/hash/4c5bcfec8584af0d967f1ab10179ca4b-Abstract.html) · [评分卡](../../leaderboard/papers/ddpm/README.md)

正向过程逐步给数据加高斯噪声，训练时随机抽噪声时刻，让网络预测混入的噪声。反向生成从纯噪声开始，多步使用网络估计均值并采样，得到图像或换成动作序列后的条件样本。原文给出变分目标与简化去噪目标的联系，在 CIFAR-10 和 LSUN 评估图像生成质量。

## 技术挂点

- [扩散去噪](../concepts/diffusion.md)：训练网络从带噪对象估计噪声或干净目标，生成时从噪声开始迭代恢复样本。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md#22-加噪公式里为什么还要把原图缩小)

- [条件生成](../concepts/generation.md)：从一个条件生成多个可能输出，学习图像、视频或动作的分布而非只给一个均值。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md#6-三个问题再落到机器人动作上)

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md#36-打开-b-区u-net-里面怎样处理图像和时间)

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md#6-三个问题再落到机器人动作上)

- [动作块](../concepts/chunk.md)：一次预测多个未来控制时刻的动作，再执行部分并用新观测更新。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/ddpm-2006.11239/README.md#6-三个问题再落到机器人动作上)

## 本篇行星与卫星

- [扩散去噪](ddpm/diffusion.md) · 已讲解
- [条件生成](ddpm/generation.md) · 已讲解
- [注意力](ddpm/attention.md) · 已讲解
- [动作表示](ddpm/action.md) · 已讲解
- [动作块](ddpm/chunk.md) · 已讲解
- [本篇方法链路](ddpm/method-chain.md) · 已讲解
- [从高概率到好看的样本](ddpm/problem.md) · 已讲解
- [前向与反向马尔可夫链](ddpm/markov.md) · 已讲解
- [图像、噪声与批形状](ddpm/shapes.md) · 已讲解
- [固定β日程](ddpm/schedule.md) · 已讲解
- [缩信号与控方差](ddpm/variance.md) · 已讲解
- [直达任意噪声等级](ddpm/marginal.md) · 已讲解
- [已知x0的高斯后验](ddpm/posterior.md) · 已讲解
- [变分账本的三部分](ddpm/elbo.md) · 已讲解
- [高斯KL与时间权重](ddpm/gaussian-kl.md) · 已讲解
- [从预测噪声到反向均值](ddpm/noise-param.md) · 已讲解
- [噪声条件均值与score](ddpm/score.md) · 已讲解
- [离散像素的高斯积分](ddpm/decoder.md) · 已讲解
- [Lsimple重分配训练权重](ddpm/simple.md) · 已讲解
- [已知答案与预测值的梯度](ddpm/gradient.md) · 已讲解
- [共享网络的反向采样](ddpm/sampling.md) · 已讲解
- [采样硬件与批量账单](ddpm/runtime.md) · 已讲解
- [U-Net特征尺度与跳连](ddpm/unet.md) · 已讲解
- [正弦时间嵌入](ddpm/time.md) · 已讲解
- [卷积残差块与GroupNorm](ddpm/residual.md) · 已讲解
- [16×16空间注意力](ddpm/spatial-attention.md) · 已讲解
- [IS、FID与NLL上界](ddpm/metrics.md) · 已讲解
- [分辨率与数据集条件](ddpm/large-image.md) · 已讲解
- [参数化与损失分开看](ddpm/ablation.md) · 已讲解
- [xhat0不是下一步状态](ddpm/estimate.md) · 已讲解
- [反向步数下的质量](ddpm/progress.md) · 已讲解
- [逐步编码与码率失真](ddpm/rate.md) · 已讲解
- [最后细节的编码成本](ddpm/late-bits.md) · 已讲解
- [共享中间状态再随机分叉](ddpm/fork.md) · 已讲解
- [信息恢复顺序与自回归](ddpm/autoregressive.md) · 已讲解
- [带噪状态插值](ddpm/interpolation.md) · 已讲解
- [动作扩散接口与执行时间](ddpm/downstream.md) · 已讲解

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
