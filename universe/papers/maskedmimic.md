# MaskedMimic 星系

MaskedMimic: Unified Physics-Based Character Control Through Masked Motion Inpainting

**导读** · 动作先验与全身技能

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/maskedmimic.md) · [原文](https://dl.acm.org/doi/10.1145/3687951) · [评分卡](../../leaderboard/papers/maskedmimic/README.md)

第一阶段用 RL 训练看到完整参考动作与场景的跟踪控制器，得到物理可执行动作。第二阶段随机遮蔽目标，把完全约束教师蒸馏成接受部分关键帧、物体与文字条件的学生，补出其余动作。验证覆盖多种约束、场景交互和任务切换，研究对象是模拟角色。

## 技术挂点

- [遮蔽预测](../concepts/masking.md)：隐藏部分输入，训练模型恢复像素、token 或表征。恢复什么决定监督重点。

- [教师学生蒸馏](../concepts/distill.md)：用教师的预测或动作监督学生，让部署模型复制可用行为。

- [动作先验](../concepts/motion-prior.md)：从运动数据学习自然动作规律，再把它接进物理控制或技能选择。

## 本篇行星与卫星

- [遮蔽预测](maskedmimic/masking.md) · 初读挂点
- [教师学生蒸馏](maskedmimic/distill.md) · 初读挂点
- [动作先验](maskedmimic/motion-prior.md) · 初读挂点
- [本篇方法链路](maskedmimic/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
