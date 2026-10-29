# 动作损失与预见损失 · JAM

用加权未来特征误差辅助动作学习。

总目标为动作flow-matching损失加lambda乘未来特征余弦损失；梯度通过预测头回到当前骨干，而不是把未来喂给策略。

[本篇星系](../jam.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/jam.md) · [原文依据](https://arxiv.org/html/2610.37219v1)
