# Segment Anything

**SAM** · ICCV 2023 · 本版排名 5 · 综合分 **95.3 / 100**

[解读导读](../../../library/sam.md) · [具身感知与场景表示](../../../paper-map/README.md#track-embodied-perception) · [ICCV集锦](../../../venues/ICCV/README.md)

[原文](https://openaccess.thecvf.com/content/ICCV2023/html/Kirillov_Segment_Anything_ICCV_2023_paper.html) · [PDF](https://openaccess.thecvf.com/content/ICCV2023/papers/Kirillov_Segment_Anything_ICCV_2023_paper.pdf) · [阅读卡片](../../../library/sam.md)

论文出处：[Alexander Kirillov / Eric Mintun 等4位 · Meta FAIR](../../origins/papers/sam.md)

## 机制简析

图像编码器先算一次图像特征，点、框或已有掩码由提示编码器表达，轻量掩码解码器联合两者预测目标区域。一次图像编码可以服务多次交互，模型同时输出多个候选以应对提示歧义。数据引擎让模型辅助人工标注再改进模型，原文以零样本图像分割和不同提示任务验证迁移。

带着这个问题读：给视觉系统一个点或框，它怎样找到目标轮廓，哪些信息还需要控制策略来补？

初读判断：任务、模型和数据闭环连得清楚，大规模公开数据与跨域实验充足；读者能看懂分割接口怎样进入机器人感知链。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 90 | 20% |
| 实验与证据 | 96 | 20% |
| 学术影响 | 100 | 10% |
| 近期关注 | 100.0 | 5% |
| 复用价值 | 99 | 8% |
| 阅读价值 | 95 | 7% |

刊会依据：[ICCV 2023](../../../venues/ICCV/README.md)，正式出处见[出版/原文记录](https://openaccess.thecvf.com/content/ICCV2023/html/Kirillov_Segment_Anything_ICCV_2023_paper.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；正式刊会版本；匹配题目：Segment Anything。累计被引 **10791**，2025–2026 被引 **7657**；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4390874575) · [文献计量条目](https://openalex.org/W4390874575)

### 影响与关注的计算依据

- **学术影响 100**：身份匹配的累计引用C=10791，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4390874575)
- **近期关注 100.0**：近期已定位引用R=7657；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W4390874575)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/facebookresearch/segment-anything) | GitHub Star 54980；GitHub Watch订阅 338；GitHub Fork 6378 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/facebook/sam-vit-huge) | HF 最近30天下载 315565；HF 仓库累计点赞 199 | 单篇原研究权重的HF转换版，按此仓库统计；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2304.02643) | HF 论文累计点赞 6 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
