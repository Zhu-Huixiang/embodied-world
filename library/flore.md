# Learning Force-Reactive Humanoid Loco-Manipulation

**解读导读** · arXiv 2026 · [操作与动作块](../paper-map/README.md#track-manipulation)

研究范围：力反馈示范学习、双手接触操作与人形全身控制；G1三类指定接触任务。

[原文入口](https://arxiv.org/abs/2610.35862v1) · [原文 PDF](https://arxiv.org/pdf/2610.35862v1) · [作者项目 / 代码入口](https://louis-leee.github.io/FLoRe/) · [作者与团队](../leaderboard/origins/papers/flore.md)

## 先看它做了什么

双手持夹爪记录腕部图像、六轴接触力/力矩和身体运动，先做无机器人示范，再补成机器人可跟踪的全身参考。每任务一套扩散策略读取两张224×224腕图、14维相对状态和双手wrench历史，同时生成运动关键点与每手力指令；高层动作块交给低层全身控制器。低层将力误差积分换成手部位置目标偏移：命令方向持续调力，其余方向保持顺应，真实腕部传感器闭合反馈环。力不是只在训练时当标签，而是从示范、策略输入/输出一路接到执行。

## 带着什么问题读

**位置轨迹为什么还不够？力观测、力指令与全身控制各自解决哪一步，关闭一条通道会怎样？**

## 为什么值得继续读

把力标注示范、预测力指令和真实全身执行串成可检验的接口；位置基线、去力命令和去力观测分别对照，能区分到底哪条力通道有用。

证据入口：Table II：三任务、每条件每任务10次，FLoRe共24/30成功，位置DP为8/30；去力命令11/30，去力观测20/30。架构、示范数据和训练日程匹配；每任务单独训练。Table I显示跟力收益同时伴随部分root/腕位置误差增加；实机x向跟力约1.1N稳态误差、1.8s进入±1N带。

具身关联：将接触反馈与全身平衡接在同一执行链，直接服务推、转、擦等人形机器人操作。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[知识星系](../universe/papers/flore.md) · [七维评分与雷达](../leaderboard/papers/flore/README.md) · [arXiv集锦](../arxiv/README.md#paper-flore) · [地图方向](../paper-map/README.md#track-manipulation) · [首页](../README.md)

元数据核对：2026-10-28。
