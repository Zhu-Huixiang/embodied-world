# LIBERO: Benchmarking Knowledge Transfer for Lifelong Robot Learning

出处：NeurIPS 2023。研究范围：终身机器人学习基准、知识迁移与多任务操作。

[原文入口](https://proceedings.neurips.cc/paper_files/paper/2023/hash/8c3c666820ea055a77726d66fc7d447f-Abstract.html) · [原文 PDF](https://proceedings.neurips.cc/paper_files/paper/2023/file/8c3c666820ea055a77726d66fc7d447f-Paper-Datasets_and_Benchmarks.pdf) · [作者项目 / 代码入口](https://libero-project.github.io/)

NeurIPS 2023 Datasets and Benchmarks 正式轨；原论文是终身学习问题，后续 VLA 常用多任务成功率不等于原论文完整协议。

阅读问题：**一个机器人顺序学新任务时，究竟迁移的是物体概念、动作技能，还是两者的组合？**

收录理由：当前机器人策略常用公开评测基准；原论文对任务知识类型、遗忘、顺序与预训练的拆解具有长期方法价值。

证据入口：NeurIPS 正式 PDF 给出四套任务、人类示范、架构/终身算法/顺序/预训练研究，复用广且评测设计有清楚科学问题；不能只把它理解成榜单分母。

具身关联：当前机器人策略常用公开评测基准；原论文对任务知识类型、遗忘、顺序与预训练的拆解具有长期方法价值。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/libero/README.md)

机制简析：程序化构造物体、空间、目标和长任务不同组合，把迁移对象拆成概念知识与执行知识；模型按任务顺序学习，在新任务上只能有限访问旧数据。评测分别检查前向迁移、遗忘、任务顺序和预训练作用。原文比较顺序微调、回放和保留参数等办法，发现某些防遗忘方法会压制新任务学习。
<!-- discovery:end -->
