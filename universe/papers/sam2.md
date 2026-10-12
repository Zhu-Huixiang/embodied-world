# SAM 2 星系

SAM 2: Segment Anything in Images and Videos

**导读** · 具身感知与场景表示

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/sam2.md) · [原文](https://openreview.net/forum?id=Ha6RTeWMd0) · [评分卡](../../leaderboard/papers/sam2/README.md)

逐帧图像特征通过记忆注意力读取之前的目标提示与掩码信息，再与当前提示一起预测本帧掩码。记忆编码器把当前预测存入记忆，下一帧继续使用；静态图像相当于记忆为空的视频。原文比较交互次数、速度以及图像和视频分割基准。

## 技术挂点

- [空间表示](../concepts/spatial.md)：保留像素、点、体素或对象相对位置的表示，让预测能接到几何与动作位置。

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。

- [闭环滚动与历史偏移](../concepts/rollout.md)：重复预测、执行或生成，把新观测或模型历史接回后续计算。

## 本篇行星与卫星

- [空间表示](sam2/spatial.md) · 初读挂点
- [注意力](sam2/attention.md) · 初读挂点
- [闭环滚动与历史偏移](sam2/rollout.md) · 初读挂点
- [本篇方法链路](sam2/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
