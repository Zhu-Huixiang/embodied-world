# 全身控制与执行

将运动目标、机器人状态和约束转成关节目标或力矩，协调腿、手臂与底盘。

生成了目标之后，还要沿实际控制接口看反馈。

分类上层：[动作表示](action.md)。

## 在完整解读里看计算与例子

- [Holo-M：对应章节](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/holo-m-2609.35709/README.md#34-四阶段训练e区让缺标签的数据也能上桌)

## 哪些论文用到或讨论它

- [Holo-M](../papers/holo-m.md) · 已精讲 · [原文](https://arxiv.org/abs/2609.35709v1)
- [DeepMimic](../papers/deepmimic.md) · 机制导读 · [原文](https://xbpeng.github.io/projects/DeepMimic/)
- [Mobile ALOHA](../papers/mobile-aloha.md) · 机制导读 · [原文](https://proceedings.mlr.press/v270/fu25b.html)
- [HumanPlus](../papers/humanplus.md) · 机制导读 · [原文](https://proceedings.mlr.press/v270/fu25a.html)
- [OmniH2O](../papers/omnih2o.md) · 机制导读 · [原文](https://proceedings.mlr.press/v270/he25b.html)
- [PHC](../papers/phc.md) · 机制导读 · [原文](https://openaccess.thecvf.com/content/ICCV2023/html/Luo_Perpetual_Humanoid_Control_for_Real-time_Simulated_Avatars_ICCV_2023_paper.html)
- [Deep WBC](../papers/deep-whole-body-control.md) · 机制导读 · [原文](https://proceedings.mlr.press/v205/fu23a.html)
- [ExBody](../papers/exbody.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss20/p107.html)
- [SONIC](../papers/sonic.md) · 机制导读 · [原文](https://www.science.org/doi/10.1126/scirobotics.aed4592)
- [HOVER](../papers/hover.md) · 机制导读 · [原文](https://hover-versatile-humanoid.github.io/)
- [SuperMimic](../papers/supermimic.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.28480)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
