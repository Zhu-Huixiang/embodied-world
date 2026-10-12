# Transporter 星系

Transporter Networks: Rearranging the Visual World for Robotic Manipulation

**导读** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/transporter.md) · [原文](https://proceedings.mlr.press/v155/zeng21a.html) · [评分卡](../../leaderboard/papers/transporter/README.md)

网络先在 RGB-D 视觉空间中预测拾取区域，取出局部深层特征，再将它与整幅场景特征互相关来确定放置位置和旋转。动作输出与输入空间对应，平移和旋转结构被模型直接利用，不先构建对象姿态或分割。原文覆盖刚体、绳索和堆物推动，比较样本效率，并扩展到六自由度拾放和真实机器人。

## 技术挂点

- [空间表示](../concepts/spatial.md)：保留像素、点、体素或对象相对位置的表示，让预测能接到几何与动作位置。

- [行为克隆](../concepts/bc.md)：直接监督观测到动作的映射，不必在每次更新中根据奖励搜索。

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。

## 本篇行星与卫星

- [空间表示](transporter/spatial.md) · 初读挂点
- [行为克隆](transporter/bc.md) · 初读挂点
- [动作表示](transporter/action.md) · 初读挂点
- [本篇方法链路](transporter/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
