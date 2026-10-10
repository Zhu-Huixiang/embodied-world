# Ctrl-World: A Controllable Generative World Model for Robot Manipulation

**Ctrl-World** · ICLR 2026 · 本版排名 98 · 综合分 **76.9 / 100**

[解读导读](../../../library/ctrl-world.md) · [世界模型与模型强化学习](../../../paper-map/README.md#track-world-model) · [ICLR集锦](../../../venues/ICLR/README.md)

[原文](https://proceedings.iclr.cc/paper_files/paper/2026/hash/0ae94013da7cd459402fd77874e09ee3-Abstract-Conference.html) · [PDF](https://arxiv.org/pdf/2510.10125v1) · [阅读卡片](../../../library/ctrl-world.md)

## 机制简析

1.5B SVD初始化，多相机token联合生成；稀疏历史图像带机器人姿态通过逐帧cross-attention检索；未来动作转换笛卡尔姿态后逐帧条件化。策略在模型里闭环rollout，人工筛成功轨迹再微调VLA。

带着这个问题读：怎样让视频生成器按真实动作走，并使想象中的策略排名接近实机？

初读判断：不是只展示漂亮视频：三模块消融、256条十秒片段、三种公开策略七类任务和真实回训建立了闭环价值。模型对碰撞、滑动、旋转和重试仍有偏差，人工成功筛选的成本须计入；复用有官方实现支撑。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 95.0 | 30% |
| 创新性 | 87 | 20% |
| 实验与证据 | 86 | 20% |
| 学术影响 | 0.0 | 10% |
| 近期关注 | 0.0 | 5% |
| 复用价值 | 90 | 8% |
| 阅读价值 | 94 | 7% |

刊会依据：[ICLR 2026](../../../venues/ICLR/README.md)，正式出处见[出版/原文记录](https://proceedings.iclr.cc/paper_files/paper/2026/hash/0ae94013da7cd459402fd77874e09ee3-Abstract-Conference.html)；采用2026-10-10刊会快照。


编辑深度：选题初读（方法、实验与局限）；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：Ctrl-World: A Controllable Generative World Model for Robot Manipulation。累计被引 0，2025–2026 被引 0；快照：2026-10-10T11:42:48+08:00。

[指标记录](https://api.openalex.org/works/W4415273528) · [文献计量条目](https://openalex.org/W4415273528)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
