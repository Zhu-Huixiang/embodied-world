# 生成未来视频是否是控制必需 · DreamFree

从视频生成先验到动作，关键是保留有用的预测信息。

DreamFree检验可否把冻结视频模型对未来的表征蒸馏到当前帧，省去部署时视频迭代去噪；不是取消动作去噪。

继续拆：[机器人视频域适配](df-adapt.md) · [当前帧可见性约束](df-mask.md) · [冻结的未来表征教师](df-teacher.md) · [生成流匹配正则](df-gen.md) · [冻结编码器再学动作](df-stage2.md) · [冻结特征的动作与未来探针](df-probes.md) · [LIBERO四套任务](df-libero.md) · [RoboCasa厨房任务](df-robocasa.md) · [DROID五十次实机比较](df-droid.md) · [视频可教任务组合](df-transfer.md) · [训练成本与代码状态](df-compute.md)。

[本篇星系](../dreamfree.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamfree.md) · [原文依据](https://arxiv.org/pdf/2611.04527v1)
