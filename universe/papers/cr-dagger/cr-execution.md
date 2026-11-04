# 500Hz控制闭环接住两种动作 · CR-DAgger

学习策略给参考，导纳控制器处理高频力反馈。

基策略参考与预测增量按时间对齐后相加，位置和目标wrench送入500Hz导纳控制器；base约1Hz、residual约50Hz是独立推理循环，不是三个相同的执行速率。

继续拆：[翻书：看纠正方式与力是否都需要](cr-book.md) · [皮带装配：同任务比较力与更新方式](cr-belt.md) · [齿轮插入：亚毫米接触纠正](cr-gear.md) · [布线：线材和夹具的物理变化](cr-cable.md) · [四项真实任务的证据边界](cr-scope.md)。

[本篇星系](../cr-dagger.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/cr-dagger.md) · [原文依据](https://compliant-residual-dagger.github.io/files/CR_DAgger_extended.pdf)
