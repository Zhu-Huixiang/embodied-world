# UMI 星系

Universal Manipulation Interface: In-The-Wild Robot Teaching Without In-The-Wild Robots

**导读** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/umi.md) · [原文](https://www.roboticsproceedings.org/rss20/p045.html) · [评分卡](../../leaderboard/papers/umi/README.md)

手持夹爪上的相机与位姿追踪记录人类示范，政策学习使用相对末端轨迹而非绑定某机器人底座的绝对坐标。部署时匹配观测与动作延迟，双臂任务再加入夹爪之间的相对位置，以保证示范和执行接口一致。抛掷、杯子摆放、衣物折叠与洗碗实验分别检验这些设计。

## 技术挂点

- [运动重定向](../concepts/retarget.md)：把人或另一种机器人的运动转换到目标本体的关节、末端与可达范围。

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。

- [行为克隆](../concepts/bc.md)：直接监督观测到动作的映射，不必在每次更新中根据奖励搜索。

## 本篇行星与卫星

- [运动重定向](umi/retarget.md) · 初读挂点
- [动作表示](umi/action.md) · 初读挂点
- [行为克隆](umi/bc.md) · 初读挂点
- [本篇方法链路](umi/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
