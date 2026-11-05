# 本篇方法链路 · DreamFree

先对机器人视频适配Wan，再冻结教师；学生用注意力mask让当前token只读当前观测和指令，投影成未来布局，与看过带噪真实未来的教师token做余弦蒸馏，同时保留视频流匹配正则。第二阶段冻结视觉编码器，用64个query读出预测特征，约1B动作DiT条件于指令、本体和DROID动作历史学流匹配。运行只单次视觉编码，动作仍去噪10或16步，输出32动作并执行指定前缀。

先对机器人视频适配Wan，再冻结教师；学生用注意力mask让当前token只读当前观测和指令，投影成未来布局，与看过带噪真实未来的教师token做余弦蒸馏，同时保留视频流匹配正则。第二阶段冻结视觉编码器，用64个query读出预测特征，约1B动作DiT条件于指令、本体和DROID动作历史学流匹配。运行只单次视觉编码，动作仍去噪10或16步，输出32动作并执行指定前缀。

[本篇星系](../dreamfree.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamfree.md) · [原文依据](https://arxiv.org/abs/2611.04527v1)
