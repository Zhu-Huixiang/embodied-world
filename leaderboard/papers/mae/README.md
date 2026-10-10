# Masked Autoencoders Are Scalable Vision Learners

**MAE** · CVPR 2022 · 本版排名 6 · 综合分 **95.3 / 100**

[解读导读](../../../library/mae.md) · [具身感知与场景表示](../../../paper-map/README.md#track-embodied-perception) · [CVPR集锦](../../../venues/CVPR/README.md)

[原文](https://openaccess.thecvf.com/content/CVPR2022/html/He_Masked_Autoencoders_Are_Scalable_Vision_Learners_CVPR_2022_paper.html) · [PDF](https://openaccess.thecvf.com/content/CVPR2022/papers/He_Masked_Autoencoders_Are_Scalable_Vision_Learners_CVPR_2022_paper.pdf) · [阅读卡片](../../../library/mae.md)

论文出处：[Kaiming He / Xinlei Chen · Meta FAIR](../../origins/papers/mae.md)

## 机制简析

随机遮住大部分图像 patch，编码器只处理可见部分，轻量解码器再接入 mask token 还原缺失像素。非对称结构减少昂贵编码器的计算，高遮挡比例让补全任务需要理解物体和场景。原文比较分类、检测、分割迁移；MVP 将同类编码器冻结后接到可训练控制模块。

带着这个问题读：遮住四分之三的图像后还原像素，怎样帮助机器人把预训练视觉特征用于控制？

初读判断：方法和计算节省能直接从结构理解，视觉迁移实验完整，官方实现公开；机器人实机继承关系有 MVP 原文佐证。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 91 | 20% |
| 实验与证据 | 95 | 20% |
| 学术影响 | 100 | 10% |
| 近期关注 | 100.0 | 5% |
| 复用价值 | 98 | 8% |
| 阅读价值 | 96 | 7% |

刊会依据：[CVPR 2022](../../../venues/CVPR/README.md)，正式出处见[出版/原文记录](https://openaccess.thecvf.com/content/CVPR2022/html/He_Masked_Autoencoders_Are_Scalable_Vision_Learners_CVPR_2022_paper.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；正式刊会版本；匹配题目：Masked Autoencoders Are Scalable Vision Learners。累计被引 **7952**，2025–2026 被引 **3761**；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4226002507) · [文献计量条目](https://openalex.org/W4226002507)

### 影响与关注的计算依据

- **学术影响 100**：身份匹配的累计引用C=7952，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4226002507)
- **近期关注 100.0**：近期已定位引用R=3761；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W4226002507)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/facebookresearch/mae) | GitHub Star 8361；GitHub Watch订阅 0；GitHub Fork 1345 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/facebook/vit-mae-base) | HF 最近30天下载 42967；HF 仓库累计点赞 40 | 单篇原研究权重的HF转换版，按此仓库统计；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2111.06377) | HF 论文累计点赞 6 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
