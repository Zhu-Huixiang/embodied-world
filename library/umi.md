# Universal Manipulation Interface: In-The-Wild Robot Teaching Without In-The-Wild Robots

出处：RSS 2024。研究范围：便携数据采集、相对动作与跨硬件策略接口。

[原文入口](https://www.roboticsproceedings.org/rss20/p045.html) · [原文 PDF](https://www.roboticsproceedings.org/rss20/p045.pdf) · [作者项目 / 代码入口](https://umi-gripper.github.io/)

RSS 2024。项目标注 Best Systems Paper finalist，仅写 finalist，不写获奖。

阅读问题：**拿手持夹爪采示范，怎样跨过人类手速、机器人延迟和坐标系之间的鸿沟？**

收录理由：低成本场外采集与可部署机器人策略接口的代表系统，关键设计都有明确动态/双臂实验落点。

证据入口：RSS 正式版与项目包含延迟匹配、相对动作、双夹爪信息的消融和跨硬件实机任务，开放硬件与软件教程，兼具创新和传播价值。

具身关联：低成本场外采集与可部署机器人策略接口的代表系统，关键设计都有明确动态/双臂实验落点。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/umi/README.md)

机制简析：手持夹爪上的相机与位姿追踪记录人类示范，政策学习使用相对末端轨迹而非绑定某机器人底座的绝对坐标。部署时匹配观测与动作延迟，双臂任务再加入夹爪之间的相对位置，以保证示范和执行接口一致。抛掷、杯子摆放、衣物折叠与洗碗实验分别检验这些设计。
<!-- discovery:end -->
