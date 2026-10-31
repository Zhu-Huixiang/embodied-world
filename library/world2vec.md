# world2vec: Mechanistic world models through latent dynamics learning

**解读导读** · arXiv 2026 · [世界模型与模型强化学习](../paper-map/README.md#track-world-model)

研究范围：无奖励潜动力学、目标观测MPC与可解释系统辨识；三项简化视觉仿真及71个非视觉混沌系统。

[原文入口](https://arxiv.org/abs/2610.40637v1) · [原文 PDF](https://arxiv.org/pdf/2610.40637v1) · [作者项目 / 代码入口](https://worldmodels.science/world2vec/) · [作者与团队](../leaderboard/origins/papers/world2vec.md)

## 先看它做了什么

world2vec用三帧观测编码潜状态，MLP预测动作条件变化率，以Euler残差积分出多步潜轨迹；把每一步预测对齐真实未来编码，以SIGReg或DCL防止表示塌缩。超参选择用未来检索EQA，另报告跨seed仿射一致性和LRC。执行时编码目标观测，CEM按潜距离选动作并滚动重规划，不训练奖励模型。科学辨识实验另将向量场换成稀疏多项式库，在已知最高阶和仿射坐标不确定性下读出动力学关系。

## 带着什么问题读

**世界模型拿高回报，就等于真的学会物理规律了吗？把下一状态预测换成潜速度场，再沿自己的预测轨迹训练，能让控制与动力学忠实度一起提高吗？**

## 为什么值得继续读

把任务回报、潜表示自洽和动力学恢复拆开。多步视野/连续残差/潜维消融、LeWM原规划协议和受控混合系统提供机制证据；收录为有边界的机制型预印本，保留控制比较差异及符号实验验证集报告限制。

证据入口：Table1：DCL在Pendulum/Reacher/CartPole回报826/895/232，DreamerV3为668/792/899，TD-MPC2为911/744/894（最大1000）；视觉CartPole仍失败。在线奖励训练与离线随机数据、25/8.3/5Hz控制频率不同，不能视为同预算全面超越。Table2：LeWM协议下25Hz DCL的200步目标成功80.2±1.6%，LeWM52.9±3.8%；25步目标86.2±1.1%与81.6±2.4%，对应规划2.55与8.64秒/episode。Table4固定K20、d32时DCL离散/连续LRC50.9/94.3、EQA10.6/71.1。Table3每格重选潜维/正则，且Tables3/4与Table1 LRC协议不同。71 attractor实验在validation选参并报告validation；SINDy已知最高多项式阶数，图7c经择优及真实状态仿射对齐，不当held-out泛化或盲发现物理定律。

具身关联：面向像素观测的无奖励视觉规划，连接JEPA/LeWM、Neural ODE、系统辨识与MPC；实证限于简化仿真。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[知识星系](../universe/papers/world2vec.md) · [七维评分与雷达](../leaderboard/papers/world2vec/README.md) · [arXiv集锦](../arxiv/README.md#paper-world2vec) · [地图方向](../paper-map/README.md#track-world-model) · [首页](../README.md)

元数据核对：2026-10-31。
