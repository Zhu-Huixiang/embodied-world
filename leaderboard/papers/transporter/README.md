# Transporter Networks: Rearranging the Visual World for Robotic Manipulation

本版阅读优先顺序：53；综合分：85.4 / 100；已评分权重：100%。

[原文](https://proceedings.mlr.press/v155/zeng21a.html) · [PDF](https://proceedings.mlr.press/v155/zeng21a/zeng21a.pdf) · [阅读卡片](../../../library/transporter.md)

## 机制简析

网络先在 RGB-D 视觉空间中预测拾取区域，取出局部深层特征，再将它与整幅场景特征互相关来确定放置位置和旋转。动作输出与输入空间对应，平移和旋转结构被模型直接利用，不先构建对象姿态或分割。原文覆盖刚体、绳索和堆物推动，比较样本效率，并扩展到六自由度拾放和真实机器人。

带着这个问题读：操作物体不一定要先识别物体？空间特征之间的匹配怎么直接长出动作？

初读判断：CoRL 正式版给出多种操作任务和真实验证，作者开放 Ravens、数据、模型及代码；CLIPort 原文和项目明确继承这一机制，可追溯的路线影响足以支持年限例外。

## 七维评分

![七维雷达：加载时展开一次，随后静止](radar.gif)

打开时从中心展开一次，结束后保持最终形状。[直接查看静态图](radar.svg)。加载与再次打开的播放时机取决于浏览器缓存。

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 刊会质量 | 90.0 | 30% |
| 创新性 | 96 | 20% |
| 实验与证据 | 92 | 20% |
| 学术影响 | 46.1 | 10% |
| 近期关注 | 31.3 | 5% |
| 复用价值 | 98 | 8% |
| 阅读价值 | 97 | 7% |

刊会依据：[CoRL 2020](../../../venues/CoRL/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v155/zeng21a.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：Transporter Networks: Rearranging the Visual World for Robotic Manipulation。累计被引 39，2025–2026 被引 6；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W3096099141) · [文献计量条目](https://openalex.org/W3096099141)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
