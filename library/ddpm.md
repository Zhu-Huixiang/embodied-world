# Denoising Diffusion Probabilistic Models

出处：NeurIPS 2020。研究范围：生成/表征基础，Diffusion Policy 与视频扩散的去噪建模起点。

[原文入口](https://proceedings.neurips.cc/paper/2020/hash/4c5bcfec8584af0d967f1ab10179ca4b-Abstract.html) · [原文 PDF](https://proceedings.neurips.cc/paper/2020/file/4c5bcfec8584af0d967f1ab10179ca4b-Paper.pdf) · [作者项目 / 代码入口](https://hojonathanho.github.io/diffusion/)

NeurIPS 2020 原始 DDPM；图像生成指标与下游动作成功率各按对应论文记录。

阅读问题：**加噪声再预测噪声的训练目标，怎样变成一段机器人动作的采样算法？**

收录理由：动作扩散和视频扩散共享前向加噪、条件噪声预测及反向采样这条核心链路，先读能解释具身策略到底在优化什么。

证据入口：概率建模与易训练目标的连接清楚，生成基准与目标消融可读，官方代码公开；其动作建模继承关系直接。

具身关联：动作扩散和视频扩散共享前向加噪、条件噪声预测及反向采样这条核心链路，先读能解释具身策略到底在优化什么。

经典保留理由：2020 年经典例外：现代动作扩散及视频扩散直接建立在 DDPM 类型的噪声预测和反向采样上。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/ddpm/README.md)

机制简析：正向过程逐步给数据加高斯噪声，训练时随机抽噪声时刻，让网络预测混入的噪声。反向生成从纯噪声开始，多步使用网络估计均值并采样，得到图像或换成动作序列后的条件样本。原文给出变分目标与简化去噪目标的联系，在 CIFAR-10 和 LSUN 评估图像生成质量。
<!-- discovery:end -->
