# Transformer

用注意力交换 token 信息，再逐位置加工。token 可以来自字词、图像块、状态或动作。

不同遮罩决定哪些位置能读到哪些信息。

继续拆：[注意力](attention.md) · [视觉 patch token](patches.md)。

## 哪些论文用到或讨论它

- [Transformer](../papers/attention.md) · 机制导读 · [原文](https://papers.nips.cc/paper/2017/hash/3f5ee243547dee91fbd053c1c4a845aa-Abstract.html)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
