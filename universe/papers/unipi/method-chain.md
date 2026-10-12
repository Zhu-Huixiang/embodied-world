# 本篇方法链路 · UniPi

当前图像和文字任务条件送入视频扩散模型，生成未来画面序列作为计划；逆动力学模型再从相邻或计划帧回归环境专用动作。计划能先生成稀疏关键帧再细化，也可在采样时施加额外约束。原文在组合泛化、多任务与层级规划上评估，并探索互联网视频知识迁移。

当前图像和文字任务条件送入视频扩散模型，生成未来画面序列作为计划；逆动力学模型再从相邻或计划帧回归环境专用动作。计划能先生成稀疏关键帧再细化，也可在采样时施加额外约束。原文在组合泛化、多任务与层级规划上评估，并探索互联网视频知识迁移。

[本篇星系](../unipi.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/unipi.md) · [原文依据](https://proceedings.neurips.cc/paper_files/paper/2023/hash/1d5b9233ad716a43be5c0d3023cb82d0-Abstract-Conference.html)
