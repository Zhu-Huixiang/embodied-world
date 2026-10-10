# Perpetual Humanoid Control for Real-time Simulated Avatars

出处：ICCV 2023。研究范围：物理人形动作跟踪与恢复；模拟角色基础。

[原文入口](https://openaccess.thecvf.com/content/ICCV2023/html/Luo_Perpetual_Humanoid_Control_for_Real-time_Simulated_Avatars_ICCV_2023_paper.html) · [原文 PDF](https://openaccess.thecvf.com/content/ICCV2023/papers/Luo_Perpetual_Humanoid_Control_for_Real-time_Simulated_Avatars_ICCV_2023_paper.pdf) · [作者项目 / 代码入口](https://www.zhengyiluo.com/PHC-Site/)

ICCV 2023 正式论文；实验对象为模拟 avatar。

阅读问题：**动作库越来越大，跟踪控制器怎样扩容、处理噪声并在摔倒后接着跑？**

收录理由：大规模动作跟踪与跌倒恢复基础，OmniH2O 正式论文沿用其跟踪评估和相关方法脉络，是读人形运动控制的重要入口。

证据入口：正式 ICCV，多数据集、无外部稳定力条件与恢复消融明确；后续人形全身控制继续引用和使用其评测脉络。

具身关联：大规模动作跟踪与跌倒恢复基础，OmniH2O 正式论文沿用其跟踪评估和相关方法脉络，是读人形运动控制的重要入口。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/phc/README.md)

机制简析：目标条件的物理控制器接收参考姿态或关键点，输出仿真动作以保持平衡并跟踪。渐进乘性策略按难动作扩展容量，保留已有跟踪技能，再加入失败状态恢复，避免新增任务覆盖旧技能。实验对比大规模动作跟踪、噪声姿态与跌倒恢复。
<!-- discovery:end -->
