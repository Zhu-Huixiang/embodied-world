# VideoVLA 星系

VideoVLA: Video Generators Can Be Generalizable Robot Manipulators

**导读** · 视频动作模型与视觉推理

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/videovla.md) · [原文](https://proceedings.neurips.cc/paper_files/paper/2025/hash/89a3b655a8b68ae1c76b768152c9c19d-Abstract-Conference.html) · [评分卡](../../leaderboard/papers/videovla/README.md)

以视频生成器的时空动态先验联合预测未来画面与机器人动作，考察未见操作泛化。

## 技术挂点

- [世界动作联合建模](../concepts/wam.md)：把未来状态或视频与动作放进联合条件生成过程，让视觉动态和行动相互约束。

- [视频时序生成](../concepts/video.md)：同时表达画面内容与时间变化，用历史与条件产生连续帧。

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。

## 本篇行星与卫星

- [世界动作联合建模](videovla/wam.md) · 初读挂点
- [视频时序生成](videovla/video.md) · 初读挂点
- [动作表示](videovla/action.md) · 初读挂点
- [本篇方法链路](videovla/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
