# 预测查询回合的下一关键帧 · JEDI

预测目标属于当前query，不是重建那条示范本身。

4层宽512预测器以slots、query观测和proprioception预测冻结V-JEPA2.1 ViT-L的两帧关键帧目标，256patch×1024；目标间隔不作为输入。

继续拆：[事件和速度定义关键阶段](jd-keyframes.md) · [阻止观测支路独自消化辅助损失](jd-stop-gradient.md) · [任务与过程反事实负样本](jd-negatives.md) · [示范间预测一致性筛选](jd-context-selection.md)。

[本篇星系](../jedi.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/jedi.md) · [原文依据](https://arxiv.org/pdf/2610.40356v1)
