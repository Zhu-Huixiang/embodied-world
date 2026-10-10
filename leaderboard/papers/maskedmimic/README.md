# MaskedMimic: Unified Physics-Based Character Control Through Masked Motion Inpainting

**MaskedMimic** · SIGGRAPH / TOG 2024 · 本版排名 67 · 综合分 **84.3 / 100**

[解读导读](../../../library/maskedmimic.md) · [动作先验与全身技能](../../../paper-map/README.md#track-motion-priors) · [SIGGRAPH / TOG集锦](../../../venues/SIGGRAPH-TOG/README.md)

[原文](https://dl.acm.org/doi/10.1145/3687951) · [PDF](https://xbpeng.github.io/projects/MaskedMimic/MaskedMimic_2024.pdf) · [阅读卡片](../../../library/maskedmimic.md)

论文出处：[Chen Tessler · NVIDIA / Bar-Ilan University 等3个出处](../../origins/papers/maskedmimic.md)

## 机制简析

第一阶段用 RL 训练看到完整参考动作与场景的跟踪控制器，得到物理可执行动作。第二阶段随机遮蔽目标，把完全约束教师蒸馏成接受部分关键帧、物体与文字条件的学生，补出其余动作。验证覆盖多种约束、场景交互和任务切换，研究对象是模拟角色。

带着这个问题读：把动作目标遮掉一部分，怎样训练出接受位置、文字和环境条件的统一控制器？

初读判断：TOG/SIGGRAPH Asia 正式论文，统一目标表示与多控制入口实验完整，公开资源为人形控制的动作先验研究提供复用基础。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 90.4 | 30% |
| 创新性 | 94 | 20% |
| 实验与证据 | 88 | 20% |
| 学术影响 | 46.4 | 10% |
| 近期关注 | 43.3 | 5% |
| 复用价值 | 92 | 8% |
| 阅读价值 | 95 | 7% |

刊会依据：[SIGGRAPH / TOG 2024](../../../venues/SIGGRAPH-TOG/README.md)，正式出处见[出版/原文记录](https://dl.acm.org/doi/10.1145/3687951)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；正式刊会版本；匹配题目：MaskedMimic: Unified Physics-Based Character Control Through Masked Motion Inpainting。累计被引 **40**，2025–2026 被引 **40**；快照：2026-10-10T09:51:57+08:00。

[指标记录](https://api.openalex.org/works/W4404526366) · [文献计量条目](https://openalex.org/W4404526366)

### 影响与关注的计算依据

- **学术影响 46.4**：身份匹配的累计引用C=40，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4404526366)
- **近期关注 43.3**：近期已定位引用R=40；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W4404526366)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/NVlabs/ProtoMotions) | GitHub Star 2429；GitHub Watch订阅 60；GitHub Fork 449 | 多论文/多模型共享仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2409.14393) | HF 论文累计点赞 9 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
