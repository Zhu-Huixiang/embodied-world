# 固定权重下的任务配置适应 · JEDI

测试时换任务示范来改变策略行为，模型权重保持固定。

任务配置τ包含目标、物体集合和场景；支持集C由N条该配置的示范组成，查询回合从新的初始状态执行。测试配置未参与训练，但共享已见运动原语。这里检验的是目标、布局和执行过程的上下文适应，不是未知地形或动力学参数识别；人类视频实机接口仍先经过同平台posttraining。

[本篇星系](../jedi.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/jedi.md) · [原文依据](https://arxiv.org/pdf/2610.40356v1)
