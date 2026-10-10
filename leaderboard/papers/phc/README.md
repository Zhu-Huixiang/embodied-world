# Perpetual Humanoid Control for Real-time Simulated Avatars

**PHC** · ICCV 2023 · 本版排名 41 · 综合分 **87.5 / 100**

[原文](https://openaccess.thecvf.com/content/ICCV2023/html/Luo_Perpetual_Humanoid_Control_for_Real-time_Simulated_Avatars_ICCV_2023_paper.html) · [PDF](https://openaccess.thecvf.com/content/ICCV2023/papers/Luo_Perpetual_Humanoid_Control_for_Real-time_Simulated_Avatars_ICCV_2023_paper.pdf) · [阅读卡片](../../../library/phc.md)

## 机制简析

目标条件的物理控制器接收参考姿态或关键点，输出仿真动作以保持平衡并跟踪。渐进乘性策略按难动作扩展容量，保留已有跟踪技能，再加入失败状态恢复，避免新增任务覆盖旧技能。实验对比大规模动作跟踪、噪声姿态与跌倒恢复。

带着这个问题读：动作库越来越大，跟踪控制器怎样扩容、处理噪声并在摔倒后接着跑？

初读判断：正式 ICCV，多数据集、无外部稳定力条件与恢复消融明确；后续人形全身控制继续引用和使用其评测脉络。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 95.0 | 30% |
| 创新性 | 90 | 20% |
| 实验与证据 | 90 | 20% |
| 学术影响 | 54.4 | 10% |
| 近期关注 | 66.4 | 5% |
| 复用价值 | 96 | 8% |
| 阅读价值 | 94 | 7% |

刊会依据：[ICCV 2023](../../../venues/ICCV/README.md)，正式出处见[出版/原文记录](https://openaccess.thecvf.com/content/ICCV2023/html/Luo_Perpetual_Humanoid_Control_for_Real-time_Simulated_Avatars_ICCV_2023_paper.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：正式刊会版本；OpenAlex题目：Perpetual Humanoid Control for Real-time Simulated Avatars。累计被引 77，2025–2026 被引 61；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W4390874171) · [文献计量条目](https://openalex.org/W4390874171)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
