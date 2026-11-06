# 先按接触类型训练三类专家 · HALO

移动/穿障、推物、坐下分别训练PPO专家，避免奖励尺度与接触差异互相拖累。

移动族含GO-TO、DOOR、CROUCH、CRAWL及重定向运动；专家使用特权状态、17×11局部高度图、10帧参考与30步历史，按失败率增加难转接采样。

继续拆：[把正确专家路由给当前技能](halo-distill.md)。

[本篇星系](../halo.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/halo.md) · [原文依据](https://arxiv.org/pdf/2611.06908v1)
