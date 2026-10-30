# Differentiable Contact Dynamics for Legged Locomotion: Policy Learning and Contact-Implicit Trajectory Optimization

**DiffContact** · arXiv 2026 · 本版排名 111 · 综合分 **65.8 / 100**

[解读导读](../../../library/diffcontact.md) · [Locomotion 与运动适应](../../../paper-map/README.md#track-locomotion) · [arXiv集锦](../../../arxiv/README.md#paper-diffcontact)

[知识星系](../../../universe/papers/diffcontact.md) · [原文](https://arxiv.org/abs/2610.35852v1) · [PDF](https://arxiv.org/pdf/2610.35852v1) · [阅读卡片](../../../library/diffcontact.md)

论文出处：[**Gijeong Kim**](../../origins/papers/diffcontact.md)<br>[韩国科学技术院（KAIST）](../../origins/papers/diffcontact.md)

## 机制简析

前向继续用硬接触模拟器生成轨迹，只在反向替换接触冲量的敏感度。方法对含de Saxcé修正的库仑摩擦二阶锥互补条件做完整锥中心路径松弛，从硬接触解出发用Newton迭代找到反向求导的评估点，组装状态/动作转移Jacobian，再供BPTT更新策略或DDP/iLQR优化轨迹。法向与切向一起松弛，梯度才有机会指向离地、粘住和滑动这些邻近模式；松弛参数趋零时回到固定接触模式的精确敏感度。

带着这个问题读：脚从粘地到滑动，精确梯度为何可能指不出路？保留硬接触前向、只松弛反向梯度，能换来什么又付出什么？

初读判断：创新90：把硬接触前向与完整摩擦锥松弛反向解耦，明确补上仅法向松弛欠缺的切向跨模式信息。证据88：三种梯度同前向比较、10种子学习评估、PPO样本/耗时对照、Newton残差和锥可行性审计，外加45kg四足无微调实机。训练目标/估计器与PPO并不相同，CITO主要仿真，点足平地模型也限制外推。复用70：推导、算法与附录超参较全，仍需解析刚体导数和接触求解工程。阅读94：适合解释为什么“模拟器能求导”不自动等于“接触梯度能把策略带对”。影响与关注另计。

## 七维评分

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="radar-dark.gif">
  <img src="radar.gif" alt="透明七维雷达，展开一次后静止" width="760">
</picture>

[透明静态图](radar.svg) · [深色静态图](radar-dark.svg)

| 维度 | 分数 / 100 | 权重 |
| --- | --- | --- |
| 公开与评审 | 60 | 30% |
| 创新性 | 90 | 20% |
| 实验与证据 | 88 | 20% |
| 学术影响 | 0 | 10% |
| 近期关注 | 0 | 5% |
| 复用价值 | 70 | 8% |
| 阅读价值 | 94 | 7% |

公开与评审依据：arXiv v1完整公开，稳定论文身份、作者和时间可追溯，按完整公开阶段60计；当前阶段为预印本公开。


编辑深度：arXiv v1方法/全部实验与相关附录初读，非完整精讲；评分记录：2026-10-28。

累计引用与近期引用尚未匹配；原始值保留null。下面列出已定位的评分信号。

### 影响与关注的计算依据

- **学术影响 0**：本次有界补查未核到独立研究采用，按独立采用量表起点0计；引用接口受限/尚未匹配，原始引用为null，这个分数不等于被引0。 [依据1](https://arxiv.org/abs/2610.35852v1) · [依据2](https://api.github.com/search/repositories?q=2610.35852&per_page=10) · [依据3](https://huggingface.co/api/papers/2610.35852)
- **近期关注 0**：本次未取得可核的单篇平台计数或近期独立技术采用，按证据量表起点0计；自动摘要转载与共享索引不赋关注分，不能据此说论文无人关注。 [依据1](https://arxiv.org/abs/2610.35852v1) · [依据2](https://api.github.com/search/repositories?q=2610.35852&per_page=10) · [依据3](https://huggingface.co/api/papers/2610.35852)

零分表示本次快照已定位的信号处在量表起点；创新和实验两轴分别评价方法。

### 论文公开入口与传播快照

- [project 入口](https://diffcontact.github.io)

[传播数据与采用依据](../../social-signals.json)保留归属、统计窗口与计分信号。
[评分说明](../../methodology.md) · [返回具身榜](../../README.md) · [论文地图](../../../paper-map/README.md)
