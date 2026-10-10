# Learning Transferable Visual Models From Natural Language Supervision

**CLIP** · ICML 2021 · 本版排名 1 · 综合分 **96.4 / 100**

[解读导读](../../../library/clip.md) · [具身感知与场景表示](../../../paper-map/README.md#track-embodied-perception) · [ICML集锦](../../../venues/ICML/README.md)

[原文](https://proceedings.mlr.press/v139/radford21a.html) · [PDF](https://proceedings.mlr.press/v139/radford21a/radford21a.pdf) · [阅读卡片](../../../library/clip.md)

## 机制简析

图像编码器和文本编码器分别输出向量，经投影与归一化后计算一个批次中全部图文配对的相似度矩阵。对称交叉熵把真实配对拉近，把批内错配分开；测试时用文本描述生成类别向量，从而做零样本分类。原文在三十余个视觉数据集测试迁移，CLIPort 再将其语义特征与空间操作分支融合。

带着这个问题读：图像和一句指令怎样对齐，语义相似为什么还不能直接给出抓取位置？

初读判断：图文训练目标和零样本接口清楚，多数据集迁移实验充分，官方模型公开；机器人引用关系已由 CLIPort 原文核实。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 发表与刊会 | 95.0 | 30% |
| 创新性 | 96 | 20% |
| 实验与证据 | 95 | 20% |
| 学术影响 | 100 | 10% |
| 近期关注 | 100 | 5% |
| 复用价值 | 99 | 8% |
| 阅读价值 | 97 | 7% |

刊会依据：[ICML 2021](../../../venues/ICML/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v139/radford21a.html)；采用2026-10-10刊会快照。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量版本：作者预印本/原研究索引记录；OpenAlex题目：Learning Transferable Visual Models From Natural Language Supervision。累计被引 5256，2025–2026 被引 1485；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W3135367836) · [文献计量条目](https://openalex.org/W3135367836)

[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
