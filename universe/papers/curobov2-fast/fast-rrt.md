# 有界双向并行RRT · cuRoboV2-Fast

从起点和终点轮流扩树，批量检查候选连接。

最近点查找按节点和关节分配工作；采样边的有效前缀可入树，parallel scan分配存储；搜索有节点和轮数上限。

继续拆：[粗路线不等于可执行轨迹](fast-route-validation.md)。

[本篇星系](../curobov2-fast.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/curobov2-fast.md) · [原文依据](https://arxiv.org/pdf/2611.06913v1)
