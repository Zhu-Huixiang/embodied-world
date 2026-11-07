# 视觉扰动标签不该混进动作指令 · La-JEPA

论文报告原评估器把扰动名称追加到非语言任务文字中。

8493个非语言变体恢复训练原指令，1537个刻意语言变化保留。重测统一MuJoCo3.3.2、seed0、首初始状态、10settling和各suite220/280/300/520步；NowWAM原较长预算结果不混用。错误原因目前是作者审计，未独立执行其空库中的评测代码。

[本篇星系](../la-jepa.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/la-jepa.md) · [原文依据](https://arxiv.org/pdf/2611.08156v1)
