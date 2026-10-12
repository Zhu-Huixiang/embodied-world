# CoT-VLA 星系

CoT-VLA: Visual Chain-of-Thought Reasoning for Vision-Language-Action Models

**导读** · 视频动作模型与视觉推理

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/cot-vla.md) · [原文](https://openaccess.thecvf.com/content/CVPR2025/html/Zhao_CoT-VLA_Visual_Chain-of-Thought_Reasoning_for_Vision-Language-Action_Models_CVPR_2025_paper.html) · [评分卡](../../leaderboard/papers/cot-vla/README.md)

先预测具有任务意图的未来视觉子目标，再以它为条件生成动作，把视觉推理接入控制。

## 技术挂点

- [视频时序生成](../concepts/video.md)：同时表达画面内容与时间变化，用历史与条件产生连续帧。

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。

- [因果序列建模](../concepts/causal.md)：通过遮罩只让位置读取允许的历史，避免训练时看到运行时不存在的未来。

## 本篇行星与卫星

- [视频时序生成](cot-vla/video.md) · 初读挂点
- [动作表示](cot-vla/action.md) · 初读挂点
- [因果序列建模](cot-vla/causal.md) · 初读挂点
- [本篇方法链路](cot-vla/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
