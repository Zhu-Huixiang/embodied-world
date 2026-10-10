# CoT-VLA: Visual Chain-of-Thought Reasoning for Vision-Language-Action Models

**CoT-VLA** · CVPR 2025 · 本版排名 90 · 综合分 **81.3 / 100**

[解读导读](../../../library/cot-vla.md) · [视频动作模型与视觉推理](../../../paper-map/README.md#track-video-action) · [CVPR集锦](../../../venues/CVPR/README.md)

[原文](https://openaccess.thecvf.com/content/CVPR2025/html/Zhao_CoT-VLA_Visual_Chain-of-Thought_Reasoning_for_Vision-Language-Action_Models_CVPR_2025_paper.html) · [PDF](https://openaccess.thecvf.com/content/CVPR2025/papers/Zhao_CoT-VLA_Visual_Chain-of-Thought_Reasoning_for_Vision-Language-Action_Models_CVPR_2025_paper.pdf) · [阅读卡片](../../../library/cot-vla.md)

论文出处：[Qingqing Zhao · NVIDIA / Stanford University 等3个出处](../../origins/papers/cot-vla.md)

## 机制简析

先预测具有任务意图的未来视觉子目标，再以它为条件生成动作，把视觉推理接入控制。

带着这个问题读：预测未来图像作为目标，怎样帮助随后的一小段动作？

初读判断：未来图像作为中间目标的机制值得看；初读应追图像预测与动作性能的消融。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 86 | 20% |
| 实验与证据 | 79 | 20% |
| 学术影响 | 52.1 | 10% |
| 近期关注 | 54.0 | 5% |
| 复用价值 | 73 | 8% |
| 阅读价值 | 87 | 7% |

刊会依据：[CVPR 2025](../../../venues/CVPR/README.md)，正式出处见[出版/原文记录](https://openaccess.thecvf.com/content/CVPR2025/html/Zhao_CoT-VLA_Visual_Chain-of-Thought_Reasoning_for_Vision-Language-Action_Models_CVPR_2025_paper.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：选题初读；评分记录：2026-10-10。

计量来源：OpenAlex；正式刊会版本；匹配题目：CoT-VLA: Visual Chain-of-Thought Reasoning for Vision-Language-Action Models。累计被引 **64**，2025–2026 被引 **64**；快照：2026-10-09T18:35:28+08:00。

[指标记录](https://api.openalex.org/works/W4413156213) · [文献计量条目](https://openalex.org/W4413156213)

### 影响与关注的计算依据

- **学术影响 52.1**：身份匹配的累计引用C=64，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4413156213)
- **近期关注 54.0**：近期已定位引用R=64；数量与每月引用速度各占一半，有效观察期16个月。 [依据1](https://api.openalex.org/works/W4413156213)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [huggingface](https://huggingface.co/papers/2503.22020) | HF 论文累计点赞 0 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
