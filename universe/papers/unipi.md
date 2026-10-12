# UniPi 星系

Learning Universal Policies via Text-Guided Video Generation

**导读** · 视频动作模型与视觉推理

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/unipi.md) · [原文](https://proceedings.neurips.cc/paper_files/paper/2023/hash/1d5b9233ad716a43be5c0d3023cb82d0-Abstract-Conference.html) · [评分卡](../../leaderboard/papers/unipi/README.md)

当前图像和文字任务条件送入视频扩散模型，生成未来画面序列作为计划；逆动力学模型再从相邻或计划帧回归环境专用动作。计划能先生成稀疏关键帧再细化，也可在采样时施加额外约束。原文在组合泛化、多任务与层级规划上评估，并探索互联网视频知识迁移。

## 技术挂点

- [视频时序生成](../concepts/video.md)：同时表达画面内容与时间变化，用历史与条件产生连续帧。

- [逆动力学](../concepts/inverse.md)：从状态变化或相邻画面推回可能的动作，给视频计划连接环境专用执行接口。

- [扩散去噪](../concepts/diffusion.md)：训练网络从带噪对象估计噪声或干净目标，生成时从噪声开始迭代恢复样本。

## 本篇行星与卫星

- [视频时序生成](unipi/video.md) · 初读挂点
- [逆动力学](unipi/inverse.md) · 初读挂点
- [扩散去噪](unipi/diffusion.md) · 初读挂点
- [本篇方法链路](unipi/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
