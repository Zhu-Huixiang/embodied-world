# CoT-VLA: Visual Chain-of-Thought Reasoning for Vision-Language-Action Models

本版阅读优先顺序：79；综合分：82.0 / 100；已评分权重：100%。

[原文](https://openaccess.thecvf.com/content/CVPR2025/html/Zhao_CoT-VLA_Visual_Chain-of-Thought_Reasoning_for_Vision-Language-Action_Models_CVPR_2025_paper.html) · [PDF](https://openaccess.thecvf.com/content/CVPR2025/papers/Zhao_CoT-VLA_Visual_Chain-of-Thought_Reasoning_for_Vision-Language-Action_Models_CVPR_2025_paper.pdf) · [阅读卡片](../../../library/cot-vla.md)

## 机制简析

先预测具有任务意图的未来视觉子目标，再以它为条件生成动作，把视觉推理接入控制。

带着这个问题读：预测未来图像作为目标，怎样帮助随后的一小段动作？

初读判断：未来图像作为中间目标的机制值得看；初读应追图像预测与动作性能的消融。

## 七维评分

![七维雷达：加载时展开一次，随后静止](radar.gif)

打开时从中心展开一次，结束后保持最终形状。[直接查看静态图](radar.svg)。加载与再次打开的播放时机取决于浏览器缓存。

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 刊会质量 | 95.0 | 30% |
| 创新性 | 86 | 20% |
| 实验与证据 | 79 | 20% |
| 学术影响 | 52.1 | 10% |
| 近期关注 | 67.1 | 5% |
| 复用价值 | 73 | 8% |
| 阅读价值 | 87 | 7% |

刊会依据：[CVPR 2025](../../../venues/CVPR/README.md)，正式出处见[出版/原文记录](https://openaccess.thecvf.com/content/CVPR2025/html/Zhao_CoT-VLA_Visual_Chain-of-Thought_Reasoning_for_Vision-Language-Action_Models_CVPR_2025_paper.html)；采用2026-10-10刊会快照。


编辑深度：选题初读；评分记录：2026-10-10。

计量版本：正式刊会版本；OpenAlex题目：CoT-VLA: Visual Chain-of-Thought Reasoning for Vision-Language-Action Models。累计被引 64，2025–2026 被引 64；快照：2026-10-09T18:35:28+08:00。

[指标记录](https://api.openalex.org/works/W4413156213) · [文献计量条目](https://openalex.org/W4413156213)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
