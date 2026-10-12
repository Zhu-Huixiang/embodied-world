# robomimic 星系

What Matters in Learning from Offline Human Demonstrations for Robot Manipulation

**导读** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/robomimic.md) · [原文](https://proceedings.mlr.press/v164/mandlekar22a.html) · [评分卡](../../leaderboard/papers/robomimic/README.md)

同一组操作任务上更换算法、单人或多人示范、低维或图像观测，并控制训练和评估流程，观察各因素独立造成的差异。带历史的行为克隆能处理人类动作的时序相关性；离线 RL 在机器生成数据上的表现不能直接搬到人类数据。它还检验验证损失与执行成功率不一致时，选模型会发生什么。

## 技术挂点

- [行为克隆](../concepts/bc.md)：直接监督观测到动作的映射，不必在每次更新中根据奖励搜索。

- [离线强化学习](../concepts/offline.md)：从已有轨迹学习决策，训练时不能自由去环境补齐数据外动作的后果。

- [机器人数据与评测](../concepts/data.md)：统一观测、动作、任务与评测条件，判断数据多样性如何影响泛化。

## 本篇行星与卫星

- [行为克隆](robomimic/bc.md) · 初读挂点
- [离线强化学习](robomimic/offline.md) · 初读挂点
- [机器人数据与评测](robomimic/data.md) · 初读挂点
- [本篇方法链路](robomimic/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
