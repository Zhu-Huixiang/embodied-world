# MaskedMimic: Unified Physics-Based Character Control Through Masked Motion Inpainting

**解读导读** · SIGGRAPH / TOG 2024 · [动作先验与全身技能](../paper-map/README.md#track-motion-priors)

研究范围：物理角色动作先验；为人形控制提供前置机制。

[原文入口](https://dl.acm.org/doi/10.1145/3687951) · [原文 PDF](https://xbpeng.github.io/projects/MaskedMimic/MaskedMimic_2024.pdf) · [作者项目 / 代码入口](https://research.nvidia.com/labs/par/maskedmimic/) · [作者与团队](../leaderboard/origins/papers/maskedmimic.md)

ACM 向 Crossref 登记为 ACM Transactions on Graphics 43(6)，DOI 10.1145/3687951，在线发表 2024-11-19、印刷日期 2024-12-19；作者页及正式 PDF 确认 Proc. SIGGRAPH Asia 2024。ACM landing 抓取超时，刊会元数据已由出版商 DOI 登记核验。实验是物理模拟角色。

## 先看它做了什么

第一阶段用 RL 训练看到完整参考动作与场景的跟踪控制器，得到物理可执行动作。第二阶段随机遮蔽目标，把完全约束教师蒸馏成接受部分关键帧、物体与文字条件的学生，补出其余动作。验证覆盖多种约束、场景交互和任务切换，研究对象是模拟角色。

## 带着什么问题读

**把动作目标遮掉一部分，怎样训练出接受位置、文字和环境条件的统一控制器？**

## 为什么值得继续读

把统一控制接口表述为 masked motion inpainting，具有清晰动作先验价值；HOVER 等人形路线直接借鉴其遮罩蒸馏方向。

证据入口：TOG/SIGGRAPH Asia 正式论文，统一目标表示与多控制入口实验完整，公开资源为人形控制的动作先验研究提供复用基础。

具身关联：把统一控制接口表述为 masked motion inpainting，具有清晰动作先验价值；HOVER 等人形路线直接借鉴其遮罩蒸馏方向。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/maskedmimic/README.md) · [SIGGRAPH / TOG集锦](../venues/SIGGRAPH-TOG/README.md) · [地图方向](../paper-map/README.md#track-motion-priors) · [首页](../README.md)

元数据核对：2026-10-10。
