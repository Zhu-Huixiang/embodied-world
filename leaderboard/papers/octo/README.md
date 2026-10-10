# Octo: An Open-Source Generalist Robot Policy

**Octo** · RSS 2024 · 本版排名 38 · 综合分 **87.6 / 100**

[解读导读](../../../library/octo.md) · [视觉语言动作模型 VLA](../../../paper-map/README.md#track-vla) · [RSS集锦](../../../venues/RSS/README.md)

[原文](https://www.roboticsproceedings.org/rss20/p090.html) · [PDF](https://roboticsproceedings.org/rss20/p090.pdf) · [阅读卡片](../../../library/octo.md)

论文出处：[**Dibya Ghosh / Homer Walke 等5位**](../../origins/papers/octo.md)<br>[斯坦福 IRIS 实验室 / 伯克利 RAIL 实验室 · 另2个机构](../../origins/papers/octo.md)

## 机制简析

各类任务、图像和本体感觉先由模态 tokenizer 转成 token，Transformer 主干处理后由读取头和扩散解码器产生动作块。更换机器人时，输入或输出适配器可改变，而主干保留预训练知识并微调。项目在不同平台上区分零样本运行与小数据微调，还单独检验新力传感输入和关节控制空间。

带着这个问题读：通用策略接上新摄像头、新动作空间时，哪些模块可以保留，哪些需要改？

初读判断：RSS 论文与项目给出九个平台的评估、结构和数据消融、完整开放训练及微调资源；方法创新主要在可扩展接口和组合设计，证据与复用价值突出。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 87 | 20% |
| 实验与证据 | 91 | 20% |
| 学术影响 | 59.2 | 10% |
| 近期关注 | 61.0 | 5% |
| 复用价值 | 99 | 8% |
| 阅读价值 | 94 | 7% |

刊会依据：[RSS 2024](../../../venues/RSS/README.md)，正式出处见[出版/原文记录](https://www.roboticsproceedings.org/rss20/p090.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本/原研究索引记录；匹配题目：Octo: An Open-Source Generalist Robot Policy。累计被引 **113**，2025–2026 被引 **110**；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4402353985) · [文献计量条目](https://openalex.org/W4402353985)

### 影响与关注的计算依据

- **学术影响 59.2**：身份匹配的累计引用C=113，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4402353985)
- **近期关注 61.0**：近期已定位引用R=110；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W4402353985)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/octo-models/octo) | GitHub Star 1797；GitHub Watch订阅 19；GitHub Fork 281 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2405.12213) | HF 论文累计点赞 27 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/rail-berkeley/octo-base) | HF 最近30天下载 125；HF 仓库累计点赞 26 | 单篇论文的作者发布资产；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
