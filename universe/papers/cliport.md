# CLIPort 星系

CLIPort: What and Where Pathways for Robotic Manipulation

**导读** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/cliport.md) · [原文](https://proceedings.mlr.press/v164/shridhar22a.html) · [评分卡](../../leaderboard/papers/cliport/README.md)

语义支路用 CLIP 提取 RGB 与指令概念，空间支路从 RGB-D 学习保持位置结构的特征；两路信息进入 Transporter 的拾取与放置预测。拾取位置先决定裁出哪块特征，再用互相关找到合适的放置区域。原文在多任务仿真和真实桌面上检验新物体、语义概念与少量示范。

## 技术挂点

- [对比学习](../concepts/contrastive.md)：给相关样本较高相似度，让它们在候选竞争中被找回来。图文配对是 CLIP 的监督来源。

- [空间表示](../concepts/spatial.md)：保留像素、点、体素或对象相对位置的表示，让预测能接到几何与动作位置。

- [示范模仿](../concepts/imitation.md)：从专家、人类或教师策略的行为学习动作，研究数据、表示和执行误差。

## 本篇行星与卫星

- [对比学习](cliport/contrastive.md) · 初读挂点
- [空间表示](cliport/spatial.md) · 初读挂点
- [示范模仿](cliport/imitation.md) · 初读挂点
- [本篇方法链路](cliport/method-chain.md) · 初读挂点

## 论文间的联系

- [CLIPort](cliport.md) → [CLIP](clip.md)：CLIPort 冻结 CLIP 提供语义特征，融合保留空间结构的分支。 [原文定位](https://proceedings.mlr.press/v164/shridhar22a.html)（CLIPort §4.2 semantic stream; CLIP article §8, evidence C21）。

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
