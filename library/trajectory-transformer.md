# Offline Reinforcement Learning as One Big Sequence Modeling Problem

出处：NeurIPS 2021。研究范围：轨迹世界模型与离线规划基础。

[原文入口](https://proceedings.neurips.cc/paper_files/paper/2021/hash/099fe6b0b444c23836c4a5d07346082b-Abstract.html) · [原文 PDF](https://papers.neurips.cc/paper_files/paper/2021/file/099fe6b0b444c23836c4a5d07346082b-Paper.pdf) · [作者项目 / 代码入口](https://trajectory-transformer.github.io/)

阅读问题：**状态、动作和奖励一起变成 token 后，beam search 为什么可以用来规划？**

收录理由：序列化环境动力学和规划的代表工作，可与 Decision Transformer 形成有机制差异的对读，而不是两篇 Transformer 摘要。

证据入口：完整模型/规划链路与多个控制设定，直接比较 DT、CQL 和 IQL；后续 Diffuser 改变生成方式但延续整轨迹规划问题。

具身关联：序列化环境动力学和规划的代表工作，可与 Decision Transformer 形成有机制差异的对读，而不是两篇 Transformer 摘要。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/trajectory-transformer/README.md)

机制简析：把状态和动作各维离散化，与奖励串成 token，Transformer 联合学习整段轨迹的概率。规划时用 beam search 保留高回报候选轨迹，执行第一步后重新搜索；稀疏长时序任务还可以接 IQL 的 Q 值做搜索启发。原文同时检查长预测误差、模仿、目标到达与离线 RL。
<!-- discovery:end -->
