# Demonstrating A Walk in the Park: Learning to Walk in 20 Minutes With Model-Free Reinforcement Learning

出处：RSS 2023。研究范围：实机在线 model-free RL；四足行走。

[原文入口](https://www.roboticsproceedings.org/rss19/p056.html) · [原文 PDF](https://www.roboticsproceedings.org/rss19/p056.pdf) · [作者项目 / 代码入口](https://sites.google.com/berkeley.edu/walk-in-the-park)

RSS 2023 正式篇名含 Demonstrating；不要与题名略异的早期 arXiv 版直接拼接引用。正式 PDF 作者次序 Laura Smith、Ilya Kostrikov、Sergey Levine，proceedings HTML 作者次序不同，计量优先 DOI/正式篇名。

阅读问题：**没有世界模型和动作模板，如何把实机采样与梯度更新快到足够实用？**

收录理由：和 DayDreamer 形成可讨论的实机样本效率对读：同样在线学习，走 model-free、任务与工程设计路线。

证据入口：RSS 正式论文，有真实在线学习、多地面实验和算法/系统设计分析；可与世界模型实机路线作有条件的技术比较。

具身关联：和 DayDreamer 形成可讨论的实机样本效率对读：同样在线学习，走 model-free、任务与工程设计路线。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/walk-in-the-park/README.md)

机制简析：基于 SAC/DroQ 的 actor-critic 从实机回放数据学习，用较高更新比、Dropout 和归一化稳定值函数。策略直接输出关节目标，本体传感器提供状态和奖励，异步采样训练与仔细的动作空间设计减少等待。论文在室内外多种地面验证从头学走路，并在模拟中分析设计选择。
<!-- discovery:end -->
