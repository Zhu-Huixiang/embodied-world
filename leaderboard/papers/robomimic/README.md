# What Matters in Learning from Offline Human Demonstrations for Robot Manipulation

**robomimic** · CoRL 2021 · 本版排名 41 · 综合分 **87.0 / 100**

[解读导读](../../../library/robomimic.md) · [操作与动作块](../../../paper-map/README.md#track-manipulation) · [CoRL集锦](../../../venues/CoRL/README.md)

[原文](https://proceedings.mlr.press/v164/mandlekar22a.html) · [PDF](https://proceedings.mlr.press/v164/mandlekar22a/mandlekar22a.pdf) · [阅读卡片](../../../library/robomimic.md)

论文出处：[**Ajay Mandlekar**](../../origins/papers/robomimic.md)<br>[得克萨斯大学奥斯汀分校 RPL 实验室 / 斯坦福大学](../../origins/papers/robomimic.md)

## 机制简析

同一组操作任务上更换算法、单人或多人示范、低维或图像观测，并控制训练和评估流程，观察各因素独立造成的差异。带历史的行为克隆能处理人类动作的时序相关性；离线 RL 在机器生成数据上的表现不能直接搬到人类数据。它还检验验证损失与执行成功率不一致时，选模型会发生什么。

带着这个问题读：同样的人类示范，为什么换个观测历史、数据质量或停训方式，结果会差这么多？

初读判断：正式 PDF 给出六类算法、仿真/真实多阶段任务、多随机种子及示范质量研究，开源数据与统一实现支撑公平对照；系统证据价值高于单个新网络模块。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 90.0 | 30% |
| 创新性 | 84 | 20% |
| 实验与证据 | 95 | 20% |
| 学术影响 | 60 | 10% |
| 近期关注 | 73.3 | 5% |
| 复用价值 | 99 | 8% |
| 阅读价值 | 94 | 7% |

刊会依据：[CoRL 2021](../../../venues/CoRL/README.md)，正式出处见[出版/原文记录](https://proceedings.mlr.press/v164/mandlekar22a.html)；采用2026-10-10刊会快照。


公开与评审依据：完整论文已公开，作者、日期与版本/固定论文身份可追溯，公开材料阶段计60。；正式刊会按登记量表计分，取较高阶段。


编辑深度：原文摘要/方法与实验初读；评分记录：2026-10-10。

累计引用与近期引用尚未匹配；原始值保留null。下面列出已定位的评分信号。

### 影响与关注的计算依据

- **学术影响 60**：Diffusion Policy直接使用robomimic基准与BC-RNN对照，GR00T N1继续将RoboMimic BC-Transformer列为正式基线；跨策略家族的持续采用按多个独立方法档评分。 [依据1](https://arxiv.org/pdf/2303.04137) · [依据2](https://arxiv.org/html/2503.14734v2)
- **近期关注 73.3**：huggingface 的论文专属入口：HF 最近30天下载=4646；按100000上限对数压缩。 [依据1](https://huggingface.co/api/datasets/robomimic/robomimic_datasets) · [依据2](https://huggingface.co/datasets/robomimic/robomimic_datasets/raw/main/README.md) · [依据3](https://huggingface.co/datasets/robomimic/robomimic_datasets)

### 论文公开入口与传播快照

| 平台 / 入口 | 公开计量 | 统计范围 | 快照 |
| --- | --- | --- | --- |
| [github](https://github.com/ARISE-Initiative/robomimic) | GitHub Star 1576；GitHub Watch订阅 15；GitHub Fork 430 | 多论文/多模型共享仓库；截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/datasets/robomimic/robomimic_datasets) | HF 最近30天下载 4646；HF 仓库累计点赞 4 | 单篇论文的作者发布资产；2026-09-11 至 2026-10-10（API最近30天；含首尾的日期标签，实际滚动边界未公开） / 截至2026-10-10的累计快照 | 2026-10-10 |
| [huggingface](https://huggingface.co/papers/2108.03298) | HF 论文累计点赞 0；HF 论文讨论评论累计数 0 | 按精确arXiv ID核对的单篇论文页；截至2026-10-10的累计快照 | 2026-10-10 |

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
