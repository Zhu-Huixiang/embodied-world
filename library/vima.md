# VIMA: Robot Manipulation with Multimodal Prompts

出处：ICML 2023。研究范围：多模态提示、桌面操作与系统化组合泛化评测。

[原文入口](https://proceedings.mlr.press/v202/jiang23b.html) · [原文 PDF](https://proceedings.mlr.press/v202/jiang23b/jiang23b.pdf) · [作者项目 / 代码入口](https://vimalabs.github.io/)

ICML 2023 正式版；VIMA-Bench 是仿真桌面任务，勿把仿真规模当实机证据。

阅读问题：**文字、目标图和示范视频能否作为同一种任务提示交给机器人？**

收录理由：把不同机器人任务描述统一为多模态 prompt 的重要工作，配套系统泛化协议和架构消融。

证据入口：ICML 正式版与项目给出四级泛化协议、数据/规模研究和对象 token 消融，公开基准便于后续方法比较；实机证据弱于 RT-1，证据评分体现这一点。

具身关联：把不同机器人任务描述统一为多模态 prompt 的重要工作，配套系统泛化协议和架构消融。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/vima/README.md)

机制简析：对象图像 token 与文字交错构成任务提示，再经 T5 编码；因果 Transformer 通过交叉注意力读取提示，并结合交互历史自回归输出动作。程序化生成任务按不同泛化难度拆开测试，避免只看训练分布平均成功率。原文对对象 tokenizer、提示接入方式、模型规模和数据量分别消融。
<!-- discovery:end -->
