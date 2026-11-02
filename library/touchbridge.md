# TouchBridge: Tactile-Conditioned Human-to-Robot Transfer for Dexterous Manipulation

**解读导读** · arXiv 2026 · [操作与动作块](../paper-map/README.md#track-manipulation)

研究范围：触觉辅助离线人类示范重定向与预训练VLA微调；一套双臂灵巧手、四项真实接触任务。

[原文入口](https://arxiv.org/abs/2610.40349v1) · [原文 PDF](https://arxiv.org/pdf/2610.40349v1) · [作者项目 / 代码入口](https://touchbridge2026.github.io/) · [作者与团队](../leaderboard/origins/papers/touchbridge.md)

## 先看它做了什么

TouchBridge让人类手套和Wuji灵巧手共享指尖触觉布局及腕相机视角。Tac-Retarget联合优化两手基座SE(3)与关节，匹配指尖位姿、触觉加权接触中心及活跃taxel支撑，并沿用TopoRetarget的距离加权Laplacian思想建立触觉激活的双手接触图。接触时减弱位姿跟踪，并用响应相关几何位移补偿顺应性。SAM2/ProPainter移除人手、渲染机器人外观，固定场景AprilTag消除头部相机运动后转换动作，用转换后的视觉/状态动作微调GR00T N1.7。触觉只服务离线重定向，不输入运行策略。

## 带着什么问题读

**手指位置对上了，为什么接触还是会丢？把指腹真实接触位置和跨手接触关系一起迁移，能否省去每个物体的重建与专门机器人示范？**

## 为什么值得继续读

问题明确：纯运动学匹配易丢接触，物体/仿真依赖增加采集成本。触觉接触patch与接触图提供可计算跨本体约束，控制相同示范和微调流程的两项消融支持机制；四实机任务与等量遥操对照支持有边界的预印本收录。

证据入口：Fig6：四任务各60个人类或遥操示范，每策略每任务20次实机测试。人类转换策略55/70/90/75%，均值72.5%；遥操60/75/90/85%，77.5%，相差5个百分点不等于统计等效。采集均值11.7s对81.7s，7.0倍包含失败和重置，不包含离线转换/训练总体开销。20条转换轨迹/任务在匹配初始场景下回放87.5%，与策略泛化不同。TableII：Grasp Egg Roll的20条人类示范在Isaac Sim和重建物体mesh上评估，接触误差4.667mm，DexPilot6.354、UniDex7.715；去graph6.659、去alignment7.071、kinematic-only7.540。Fig9同60示范/任务：完整72.5%，去graph48.8%，去alignment43.8%，纯运动学38.8%；DexPilot47.5、UniDex30.0。图中误差条是四任务间标准差，不是跨seed置信区间。Fig10表明预训练先验关键，不能说从零不需要机器人数据。

具身关联：把可穿戴人类示范、触觉接触约束和VLA操作微调连接起来，直接面向双手接触丰富灵巧操作。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[知识星系](../universe/papers/touchbridge.md) · [七维评分与雷达](../leaderboard/papers/touchbridge/README.md) · [arXiv集锦](../arxiv/README.md#paper-touchbridge) · [地图方向](../paper-map/README.md#track-manipulation) · [首页](../README.md)

元数据核对：2026-11-02。
