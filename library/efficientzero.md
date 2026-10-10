# Mastering Atari Games with Limited Data

出处：NeurIPS 2021。研究范围：世界模型与样本高效 RL；游戏和模拟控制基础。

[原文入口](https://proceedings.neurips.cc/paper/2021/hash/d5eca8dc3820cad9fe56a3bafda65ca1-Abstract.html) · [原文 PDF](https://proceedings.neurips.cc/paper/2021/file/d5eca8dc3820cad9fe56a3bafda65ca1-Paper.pdf) · [作者项目 / 代码入口](https://github.com/YeWR/EfficientZero)

NeurIPS 网页摘要与所读 proceedings PDF 的 Atari 汇总值不同，精讲时固定 PDF 版并逐表核数，当前卡片不引用该差异数字。

阅读问题：**只有少量交互时，潜空间树搜索为什么还需要一致性监督、价值前缀和重分析？**

收录理由：MuZero 在小样本视觉控制上的重要后续，原文有 Atari 100k、DMControl 和组件消融，官方代码提供树搜索 RL 复用入口。

证据入口：有多任务小样本基准、MuZero 对照及组件消融；代码和后续 EfficientZero V2 构成可追踪的复用路线。

具身关联：MuZero 在小样本视觉控制上的重要后续，原文有 Atari 100k、DMControl 和组件消融，官方代码提供树搜索 RL 复用入口。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/efficientzero/README.md)

机制简析：编码器把图像变成潜状态，动力学网络预测下一潜状态，MCTS 在这个模型里比较动作。EfficientZero 用预测潜状态与真实下一帧编码的一致性补强动力学监督，预测累计价值前缀，并重分析旧数据来缓解离策略目标偏差。它测试的是有限交互预算下的游戏与模拟控制效率。
<!-- discovery:end -->
