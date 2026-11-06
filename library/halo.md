# Perceptive Humanoid Motion from Simulation

**解读导读** · arXiv 2026 · [动作先验与全身技能](../paper-map/README.md#track-motion-priors)

研究范围：视觉语言条件的人形全身控制；六个预定义技能的仿真到真实迁移，以及三条有限组合任务。

[原文入口](https://arxiv.org/abs/2611.06908v1) · [原文 PDF](https://arxiv.org/pdf/2611.06908v1) · [作者项目 / 代码入口](https://apple-aiml-research.github.io/ml-halo/) · [作者与团队](../leaderboard/origins/papers/halo.md)

所读版本为v1。单任务与组合任务分别统计；合成回合无需逐条遥操作，运动先验仍包含人类视频、mocap、真实G1终点日志和手工关键帧。

## 先看它做了什么

HALO先用INFINIGEN房间、KIMODO约束运动、场景摆放和第一视角渲染合成162698回合/296.3小时的视觉—指令—全身轨迹。冻结Qwen3.5-2B编码224×224RGB与文字，8层DiT以流匹配生成150×36的五秒骨盆相对计划；首15帧保持干净，学习接续135帧，并以15步Euler、约3Hz异步更新。低层先训练三类特权PPO专家，再按技能路由BC/DAgger蒸馏为深度学生，最后多critic PPO微调。共享跟踪器融合48×84深度、30步本体历史和计划，以50Hz输出29关节目标。上层VLM从自由语言选择有限技能并检查完成/重试，默认两台机载计算机协作。

## 带着什么问题读

**机器人会做动作，为何到了陌生客厅还是不会坐？把大规模仿真监督、语义运动生成和深度跟踪分层，能否同时补上看懂目标与处理身体接触两道缺口？**

## 为什么值得继续读

问题具体，数据合成、异步流匹配与三阶段感知跟踪的接口可逐项核对；360次实机单任务、30次实机组合任务及四组仿真消融支持有限技能sim-to-real贡献。按预印本初读收录，任务库与人工运动种子保留为适用范围。

证据入口：TableII六技能100仿真环境×10次=每技能1000次、6实机环境×10次=每技能60次；共6000/360次。实机GO-TO/SIT/DOOR/CROUCH/CRAWL/PUSH为92/85/93/100/90/88%，均值91%。三链另做1500仿真与30实机：实机100/60/50%，均值70%，只在1环境。TableIII均为SIT保留仿真100×10：房间1000/100/10/1得到84/81/64/43%；训练RTC/推理RTC/无RTC为84/66/24%；flow84对regression19，深度84对无深度74。回归替换也失去RTC，差值不是纯流匹配因果收益；TableI跨论文能力比较并非同协议数值baseline。无实机消融、seed或置信区间。

具身关联：把语言和陌生环境视觉接到人形身体的运动学参考与近身接触控制，直接讨论全身技能数据、感知跟踪和sim-to-real代价。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[知识星系](../universe/papers/halo.md) · [七维评分与雷达](../leaderboard/papers/halo/README.md) · [arXiv集锦](../arxiv/README.md#paper-halo) · [地图方向](../paper-map/README.md#track-motion-priors) · [首页](../README.md)

元数据核对：2026-11-06。
