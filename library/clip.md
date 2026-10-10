# Learning Transferable Visual Models From Natural Language Supervision

**解读导读** · ICML 2021 · [具身感知与场景表示](../paper-map/README.md#track-embodied-perception)

研究范围：生成/表征基础，开放词汇机器人感知与语言条件操作的语义先验。

[原文入口](https://proceedings.mlr.press/v139/radford21a.html) · [原文 PDF](https://proceedings.mlr.press/v139/radford21a/radford21a.pdf) · [作者项目 / 代码入口](https://github.com/openai/CLIP) · [作者与团队](../leaderboard/origins/papers/clip.md)

ICML 2021，PMLR 139；CLIPort 对 CLIP 语义流的直接使用另列为机器人应用证据。

## 先看它做了什么

图像编码器和文本编码器分别输出向量，经投影与归一化后计算一个批次中全部图文配对的相似度矩阵。对称交叉熵把真实配对拉近，把批内错配分开；测试时用文本描述生成类别向量，从而做零样本分类。原文在三十余个视觉数据集测试迁移，CLIPort 再将其语义特征与空间操作分支融合。

## 带着什么问题读

**图像和一句指令怎样对齐，语义相似为什么还不能直接给出抓取位置？**

## 为什么值得继续读

CLIPort 公开原文直接将冻结 CLIP 图文特征接入操作策略；此基础论文解释网络语义如何进入具身系统，关系明确。

证据入口：图文训练目标和零样本接口清楚，多数据集迁移实验充分，官方模型公开；机器人引用关系已由 CLIPort 原文核实。

具身关联：CLIPort 公开原文直接将冻结 CLIP 图文特征接入操作策略；此基础论文解释网络语义如何进入具身系统，关系明确。

经典保留理由：ICML 2021 早于 2021-10-10，因图文对齐已经直接用于 CLIPort 等机器人方法，作为经典例外。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/clip/README.md) · [ICML集锦](../venues/ICML/README.md) · [地图方向](../paper-map/README.md#track-embodied-perception) · [首页](../README.md)

元数据核对：2026-10-10。
