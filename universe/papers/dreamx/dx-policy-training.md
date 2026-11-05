# 预训练与任务微调两笔成本 · DreamX

latent生成器用约三分之一原预训练数据学习10万步，再加入动作头做任务学习。

生成器rank128 LoRA、2张H200、batch60；Action DiT在任务阶段才引入。抽屉实验两方法各3万步，但初始化和预训练数据不同。

[本篇星系](../dreamx.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamx.md) · [原文依据](https://arxiv.org/pdf/2611.05377v1)
