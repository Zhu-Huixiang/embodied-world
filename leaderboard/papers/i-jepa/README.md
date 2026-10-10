# Self-Supervised Learning from Images with a Joint-Embedding Predictive Architecture

**I-JEPA** · CVPR 2023 · 本版排名 26 · 综合分 **90.0 / 100**

[解读导读](../../../library/i-jepa.md) · [具身感知与场景表示](../../../paper-map/README.md#track-embodied-perception) · [CVPR集锦](../../../venues/CVPR/README.md)

[原文](https://openaccess.thecvf.com/content/CVPR2023/html/Assran_Self-Supervised_Learning_From_Images_With_a_Joint-Embedding_Predictive_Architecture_CVPR_2023_paper.html) · [PDF](https://openaccess.thecvf.com/content/CVPR2023/papers/Assran_Self-Supervised_Learning_From_Images_With_a_Joint-Embedding_Predictive_Architecture_CVPR_2023_paper.pdf) · [阅读卡片](../../../library/i-jepa.md)

论文出处：[**Mahmoud Assran**](../../origins/papers/i-jepa.md)<br>[Meta FAIR 研究院 / 麦吉尔大学 · 另2个机构](../../origins/papers/i-jepa.md)

## 机制简析

上下文编码器读取图像可见块，预测器根据目标位置预测多个缺失区域的表征，目标编码器生成需要拟合的监督向量。目标块足够大、上下文空间分布足够丰富，让任务偏向语义结构而非局部纹理补全。原文比较分类、目标计数、深度预测和掩码策略，后续时序 JEPA 再扩展预测对象。

带着这个问题读：世界模型必须把像素画出来吗，预测目标区域的 latent 会保留哪些可用信息？

初读判断：监督目标与掩码选择有可辨认机制，跨任务和设计消融扎实，官方代码公开；适合讲清具身世界模型里预测什么这一分歧。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 95.0 | 30% |
| 创新性 | 88 | 20% |
| 实验与证据 | 89 | 20% |
| 学术影响 | 75.2 | 10% |
| 近期关注 | 90.8 | 5% |
| 复用价值 | 92 | 8% |
| 阅读价值 | 96 | 7% |

刊会依据：[CVPR 2023](../../../venues/CVPR/README.md)，正式出处见[出版/原文记录](https://openaccess.thecvf.com/content/CVPR2023/html/Assran_Self-Supervised_Learning_From_Images_With_a_Joint-Embedding_Predictive_Architecture_CVPR_2023_paper.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

计量来源：OpenAlex；正式刊会版本；匹配题目：Self-Supervised Learning from Images with a Joint-Embedding Predictive Architecture。累计被引 **410**，2025–2026 被引 **304**；快照：2026-10-10T09:50:37+08:00。

[指标记录](https://api.openalex.org/works/W4386076428) · [文献计量条目](https://openalex.org/W4386076428)

### 影响与关注的计算依据

- **学术影响 75.2**：身份匹配的累计引用C=410，对数压缩上限3000。 [依据1](https://api.openalex.org/works/W4386076428)
- **近期关注 90.8**：huggingface 的论文专属入口：HF 最近30天下载=34720；按100000上限对数压缩。 [依据1](https://huggingface.co/api/models/facebook/ijepa_vith14_1k) · [依据2](https://huggingface.co/facebook/ijepa_vith14_1k/raw/main/README.md) · [依据3](https://huggingface.co/facebook/ijepa_vith14_1k)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/facebookresearch/ijepa) | GitHub Star 3488；GitHub Watch订阅 9；GitHub Fork 529 | 单篇论文仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/facebook/ijepa_vith14_1k) | HF 最近30天下载 34720；HF 仓库累计点赞 20 | 单篇原研究权重的HF转换版，按此仓库统计；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2301.08243) | HF 论文累计点赞 7 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
