# Perpetual Humanoid Control for Real-time Simulated Avatars

**解读导读** · ICCV 2023 · [动作先验与全身技能](../paper-map/README.md#track-motion-priors)

研究范围：物理人形动作跟踪与恢复；模拟角色基础。

[原文入口](https://openaccess.thecvf.com/content/ICCV2023/html/Luo_Perpetual_Humanoid_Control_for_Real-time_Simulated_Avatars_ICCV_2023_paper.html) · [原文 PDF](https://openaccess.thecvf.com/content/ICCV2023/papers/Luo_Perpetual_Humanoid_Control_for_Real-time_Simulated_Avatars_ICCV_2023_paper.pdf) · [作者项目 / 代码入口](https://www.zhengyiluo.com/PHC-Site/) · [作者与团队](../leaderboard/origins/papers/phc.md)

ICCV 2023 正式论文；实验对象为模拟 avatar。

## 先看它做了什么

目标条件的物理控制器接收参考姿态或关键点，输出仿真动作以保持平衡并跟踪。渐进乘性策略按难动作扩展容量，保留已有跟踪技能，再加入失败状态恢复，避免新增任务覆盖旧技能。实验对比大规模动作跟踪、噪声姿态与跌倒恢复。

## 带着什么问题读

**动作库越来越大，跟踪控制器怎样扩容、处理噪声并在摔倒后接着跑？**

## 为什么值得继续读

大规模动作跟踪与跌倒恢复基础，OmniH2O 正式论文沿用其跟踪评估和相关方法脉络，是读人形运动控制的重要入口。

证据入口：正式 ICCV，多数据集、无外部稳定力条件与恢复消融明确；后续人形全身控制继续引用和使用其评测脉络。

具身关联：大规模动作跟踪与跌倒恢复基础，OmniH2O 正式论文沿用其跟踪评估和相关方法脉络，是读人形运动控制的重要入口。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/phc/README.md) · [ICCV集锦](../venues/ICCV/README.md) · [地图方向](../paper-map/README.md#track-motion-priors) · [首页](../README.md)

元数据核对：2026-10-10。
