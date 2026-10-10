# Elucidating the Design Space of Diffusion-Based Generative Models

**EDM** · NeurIPS 2022 · 本版排名 27 · 综合分 **90.0 / 100**

[解读导读](../../../library/edm.md) · [Diffusion / Transformer 基础](../../../paper-map/README.md#track-diffusion-transformer) · [NeurIPS集锦](../../../venues/NeurIPS/README.md)

[原文](https://proceedings.neurips.cc/paper_files/paper/2022/hash/a98846e9d9cc01cfb87eb694d946ce6b-Abstract-Conference.html) · [PDF](https://proceedings.neurips.cc/paper_files/paper/2022/file/a98846e9d9cc01cfb87eb694d946ce6b-Paper-Conference.pdf) · [阅读卡片](../../../library/edm.md)

论文出处：[**Tero Karras**](../../origins/papers/edm.md)<br>[英伟达](../../origins/papers/edm.md)

## 机制简析

把扩散过程的噪声参数化、采样求解器和网络预处理分别定义，减少不同实现之间的隐性差异。网络输入、输出和训练损失按噪声尺度预调节，推理使用更合适的时间离散与高阶求解。原文同时重用旧模型更换采样器、重训网络，比较质量与网络调用次数。

带着这个问题读：同样是扩散，噪声尺度、网络预处理和数值求解器各改变了哪一层？

初读判断：模块化贡献配有重用旧网络和重新训练的对照，速度质量证据扎实，官方实现让设计取舍可操作。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 89 | 20% |
| 实验与证据 | 95 | 20% |
| 学术影响 | 67.6 | 10% |
| 近期关注 | 74.2 | 5% |
| 复用价值 | 96 | 8% |
| 阅读价值 | 94 | 7% |

刊会依据：[NeurIPS 2022](../../../venues/NeurIPS/README.md)，正式出处见[出版/原文记录](https://proceedings.neurips.cc/paper_files/paper/2022/hash/a98846e9d9cc01cfb87eb694d946ce6b-Abstract-Conference.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；正式刊会版本；匹配题目：Elucidating the Design Space of Diffusion-Based Generative Models。累计被引 **224**，2025–2026 被引 **219**；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W7133244780) · [文献计量条目](https://openalex.org/W7133244780)

### 影响与关注的计算依据

- **学术影响 67.6**：身份匹配的累计引用C=224，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W7133244780)
- **近期关注 74.2**：近期已定位引用R=219；数量与每月引用速度各占一半，有效观察期21.2567个月。 [依据1](https://api.openalex.org/works/W7133244780)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/NVlabs/edm) | GitHub Star 2003；GitHub Watch订阅 31；GitHub Fork 212 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2206.00364) | HF 论文累计点赞 18 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
