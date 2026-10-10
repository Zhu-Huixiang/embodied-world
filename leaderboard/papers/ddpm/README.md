# Denoising Diffusion Probabilistic Models

**DDPM** · NeurIPS 2020 · 本版排名 2 · 综合分 **95.9 / 100**

[解读导读](../../../library/ddpm.md) · [Diffusion / Transformer 基础](../../../paper-map/README.md#track-diffusion-transformer) · [NeurIPS集锦](../../../venues/NeurIPS/README.md)

[原文](https://proceedings.neurips.cc/paper/2020/hash/4c5bcfec8584af0d967f1ab10179ca4b-Abstract.html) · [PDF](https://proceedings.neurips.cc/paper/2020/file/4c5bcfec8584af0d967f1ab10179ca4b-Paper.pdf) · [阅读卡片](../../../library/ddpm.md)

论文出处：[Jonathan Ho · UC Berkeley](../../origins/papers/ddpm.md)

## 机制简析

正向过程逐步给数据加高斯噪声，训练时随机抽噪声时刻，让网络预测混入的噪声。反向生成从纯噪声开始，多步使用网络估计均值并采样，得到图像或换成动作序列后的条件样本。原文给出变分目标与简化去噪目标的联系，在 CIFAR-10 和 LSUN 评估图像生成质量。

带着这个问题读：加噪声再预测噪声的训练目标，怎样变成一段机器人动作的采样算法？

初读判断：概率建模与易训练目标的连接清楚，生成基准与目标消融可读，官方代码公开；其动作建模继承关系直接。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 96 | 20% |
| 实验与证据 | 92 | 20% |
| 学术影响 | 100 | 10% |
| 近期关注 | 100.0 | 5% |
| 复用价值 | 99 | 8% |
| 阅读价值 | 98 | 7% |

刊会依据：[NeurIPS 2020](../../../venues/NeurIPS/README.md)，正式出处见[出版/原文记录](https://proceedings.neurips.cc/paper/2020/hash/4c5bcfec8584af0d967f1ab10179ca4b-Abstract.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；作者预印本/原研究索引记录；匹配题目：Denoising Diffusion Probabilistic Models。累计被引 **5512**，2025–2026 被引 **1716**；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W3036167779) · [文献计量条目](https://openalex.org/W3036167779)

### 影响与关注的计算依据

- **学术影响 100**：身份匹配的累计引用C=5512，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W3036167779)
- **近期关注 100.0**：近期已定位引用R=1716；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W3036167779)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/hojonathanho/diffusion) | GitHub Star 5341；GitHub Watch订阅 24；GitHub Fork 493 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/google/ddpm-cifar10-32) | HF 最近30天下载 21960；HF 仓库累计点赞 94 | 单篇原研究权重的HF转换版，按此仓库统计；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2006.11239) | HF 论文累计点赞 9 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
