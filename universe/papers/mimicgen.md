# MimicGen 星系

MimicGen: A Data Generation System for Scalable Robot Learning using Human Demonstrations

**导读** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/mimicgen.md) · [原文](https://proceedings.mlr.press/v229/mandlekar23a.html) · [评分卡](../../leaderboard/papers/mimicgen/README.md)

源示范按对象中心子任务切段；新场景中选择源段，按对象的新位姿变换末端轨迹，再拼接并实际执行。执行成功才把状态和动作加入生成数据，而不是只复制一组数学坐标。原文逐步扩大初始状态分布、替换物体与机械臂，并比较生成示范和追加同量人类示范的策略表现。

## 技术挂点

- [机器人数据与评测](../concepts/data.md)：统一观测、动作、任务与评测条件，判断数据多样性如何影响泛化。

- [运动重定向](../concepts/retarget.md)：把人或另一种机器人的运动转换到目标本体的关节、末端与可达范围。

- [行为克隆](../concepts/bc.md)：直接监督观测到动作的映射，不必在每次更新中根据奖励搜索。

## 本篇行星与卫星

- [机器人数据与评测](mimicgen/data.md) · 初读挂点
- [运动重定向](mimicgen/retarget.md) · 初读挂点
- [行为克隆](mimicgen/bc.md) · 初读挂点
- [本篇方法链路](mimicgen/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
