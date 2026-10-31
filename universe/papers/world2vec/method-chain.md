# 本篇方法链路 · world2vec

world2vec用三帧观测编码潜状态，MLP预测动作条件变化率，以Euler残差积分出多步潜轨迹；把每一步预测对齐真实未来编码，以SIGReg或DCL防止表示塌缩。超参选择用未来检索EQA，另报告跨seed仿射一致性和LRC。执行时编码目标观测，CEM按潜距离选动作并滚动重规划，不训练奖励模型。科学辨识实验另将向量场换成稀疏多项式库，在已知最高阶和仿射坐标不确定性下读出动力学关系。

world2vec用三帧观测编码潜状态，MLP预测动作条件变化率，以Euler残差积分出多步潜轨迹；把每一步预测对齐真实未来编码，以SIGReg或DCL防止表示塌缩。超参选择用未来检索EQA，另报告跨seed仿射一致性和LRC。执行时编码目标观测，CEM按潜距离选动作并滚动重规划，不训练奖励模型。科学辨识实验另将向量场换成稀疏多项式库，在已知最高阶和仿射坐标不确定性下读出动力学关系。

[本篇星系](../world2vec.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/world2vec.md) · [原文依据](https://arxiv.org/abs/2610.40637v1)
