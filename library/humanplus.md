# HumanPlus: Humanoid Shadowing and Imitation from Humans

出处：CoRL 2024。研究范围：人形全身控制、遥操作与视觉模仿。

[原文入口](https://proceedings.mlr.press/v270/fu25a.html) · [原文 PDF](https://raw.githubusercontent.com/mlresearch/v270/main/assets/fu25a/fu25a.pdf) · [作者项目 / 代码入口](https://humanoid-ai.github.io/)

CoRL 2024；PMLR 270 论文集出版年为 2025。

阅读问题：**人做动作、机器人跟动作、再学自主任务，这三段数据链路如何接起来？**

收录理由：全栈人形学习的代表系统，动作数据到低层控制、影子遥操作到视觉技能形成可解释数据流水线。

证据入口：正式 CoRL，有真实人形、遥操作对照和任务成功率；同时覆盖全身控制与数据采集，适合正式公众号的系统解读。

具身关联：全栈人形学习的代表系统，动作数据到低层控制、影子遥操作到视觉技能形成可解释数据流水线。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/humanplus/README.md)

机制简析：用人类运动重定向数据在模拟里训练姿态条件的低层控制，再用单 RGB 相机估计操作者姿态，让实机实时跟随。跟随过程中记录机器人双目视觉和全身动作，随后用 Humanoid Imitation Transformer 做监督模仿，得到自主任务策略。原文分别评估遥操作、抗扰和多项自主任务。
<!-- discovery:end -->
