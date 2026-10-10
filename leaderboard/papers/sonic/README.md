# SONIC: Supersizing Motion Tracking for Natural Humanoid Whole-Body Control

**SONIC** · Sci. Robot. 2026 · 本版排名 74 · 综合分 **83.4 / 100**

[解读导读](../../../library/sonic.md) · [Locomotion 与运动适应](../../../paper-map/README.md#track-locomotion) · [Sci. Robot.集锦](../../../venues/Science-Robotics/README.md)

[原文](https://www.science.org/doi/10.1126/scirobotics.aed4592) · [PDF](https://arxiv.org/pdf/2511.07820v4) · [阅读卡片](../../../library/sonic.md)

论文出处：[Zhengyi Luo / Ye Yuan 等5位 · NVIDIA GEAR / NVIDIA](../../origins/papers/sonic.md)

## 机制简析

机器人/人体/稀疏混合命令分别编码到 FSQ 共享运动 token；同一控制解码器结合10步本体历史输出29关节目标，由PD执行。PPO与运动重建、token对齐和cycle损失联合训练；上游实时运动规划或VLA预测64维token与14维手关节。

带着这个问题读：动作跟踪为什么能吃进大规模人类动作数据，64维共享运动 token 又怎样让同一控制器接遥操作和全身 VLA？

初读判断：创新是可扩动作跟踪与统一控制接口的完整系统，而非参数大本身。原文三轴消融、跨数据测试、124段实机跟踪和动作空间消融较强；数据未匹配的baseline比较、10–20次任务试验和极端动作/长期安全问题限制证据分。已开训练、模型、C++/TensorRT部署与BONES-SEED子集，但21k GPU小时重训门槛仍高。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 92.7 | 30% |
| 创新性 | 92 | 20% |
| 实验与证据 | 89 | 20% |
| 学术影响 | 20.1 | 10% |
| 近期关注 | 69.3 | 5% |
| 复用价值 | 92 | 8% |
| 阅读价值 | 94 | 7% |

刊会依据：[Sci. Robot. 2026](../../../venues/Science-Robotics/README.md)，正式出处见[出版/原文记录](https://www.science.org/doi/10.1126/scirobotics.aed4592)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文机制与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；正式刊会版本；匹配题目：SONIC: Supersizing motion tracking for natural humanoid whole-body control。累计被引 **4**，2025–2026 被引 **4**；快照：2026-10-10T11:42:48+08:00。

[指标记录](https://api.openalex.org/works/W7202294264) · [文献计量条目](https://openalex.org/W7202294264)

### 影响与关注的计算依据

- **学术影响 20.1**：身份匹配的累计引用C=4，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W7202294264)
- **近期关注 69.3**：huggingface 的论文专属入口：HF 最近30天下载=2907；按100000上限对数压缩。 [依据1](https://huggingface.co/api/models/nvidia/GEAR-SONIC) · [依据2](https://huggingface.co/nvidia/GEAR-SONIC/raw/main/README.md) · [依据3](https://huggingface.co/nvidia/GEAR-SONIC)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/NVlabs/GR00T-WholeBodyControl) | GitHub Star 3723；GitHub Watch订阅 28；GitHub Fork 610 | 多论文/多模型共享仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/nvidia/GEAR-SONIC) | HF 最近30天下载 2907；HF 仓库累计点赞 77 | 单篇论文的作者发布资产；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2511.07820) | HF 论文累计点赞 0 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
