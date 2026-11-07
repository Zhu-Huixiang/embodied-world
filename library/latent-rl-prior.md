# Latent RL Priors for Data-Efficient Dexterous Manipulation

**解读导读** · arXiv 2026 · [操作与动作块](../paper-map/README.md#track-manipulation)

研究范围：同一KUKA iiwa+SHARPA手在MuJoCo Warp中的三项任务；全部视觉示范和评测都为仿真，双臂共享单臂控制器不等于跨形态迁移。

[原文入口](https://arxiv.org/abs/2611.08458v1) · [原文 PDF](https://arxiv.org/pdf/2611.08458v1) · [作者项目 / 代码入口](https://yixiaowang7.github.io/latent-rl-prior-page/) · [作者与团队](../leaderboard/origins/papers/latent-rl-prior.md)

所读v1。实验全部在MuJoCo Warp中完成；下游示范减少依赖十万条成功RL预训练轨迹。主对照的优化步数和最优checkpoint选择条件一并保留。

## 先看它做了什么

先微调SimToolReal teacher并收集100000条成功程序化姿态对齐轨迹，将特权历史经state tokenizer/Q-Former压为任务context；flow-matching动作transformer通过cross-attention读context，通过AdaLN读本体历史与flow time。视觉阶段冻结decoder，只以动作flow loss训练DINOv2-Small与视觉Q-Former，直接生成latent而不需要特权/latent标签；双臂的两组queries共同自注意力协调后，分别结合各臂本体进入共享单臂decoder。

## 带着什么问题读

**特权RL已经学会灵巧控制，少量视觉示范该学动作本身，还是只学怎样把图像接进冻结控制先验？**

## 为什么值得继续读

问题明确，动作条件与本体路径的拆分及action-only latent接口构成实质迁移设计；同结构scratch、显式桥接、模块学习率、多预算和质量/力probe支持限定于仿真的贡献。预算不等、checkpoint选择和缺实现细节已保留，不以名校/演示替代实验。

证据入口：全数据刷子4000、抬门500、双臂5000；本法抬门50和双臂1000示范超过π0.5/GR00T N1.7全数据基线。主实验本法100k优化步、VLA30k，每run末5checkpoint各256 rollout后取最高，通常3seed均值±SD。5kg抬门32.6%对π0.5 12.9%，分别50/500示范。Fig5同结构scratch和Fig5–7接口/冻结消融支持先验复用；force ridge probe8层仅是表征读出，不证明因果。全部仿真。

具身关联：直接连接特权RL控制经验、视觉模仿与动作生成，并分清视觉接入、已有控制支持及双臂协同责任。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[知识星系](../universe/papers/latent-rl-prior.md) · [七维评分与雷达](../leaderboard/papers/latent-rl-prior/README.md) · [arXiv集锦](../arxiv/README.md#paper-latent-rl-prior) · [地图方向](../paper-map/README.md#track-manipulation) · [首页](../README.md)

元数据核对：2026-11-07。
