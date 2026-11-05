# DreamFree 星系

Future Representation Distillation for Imagination-Free World Action Models

**导读** · 世界动作模型

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamfree.md) · [原文](https://arxiv.org/abs/2611.04527v1) · [评分卡](../../leaderboard/papers/dreamfree/README.md)

先对机器人视频适配Wan，再冻结教师；学生用注意力mask让当前token只读当前观测和指令，投影成未来布局，与看过带噪真实未来的教师token做余弦蒸馏，同时保留视频流匹配正则。第二阶段冻结视觉编码器，用64个query读出预测特征，约1B动作DiT条件于指令、本体和DROID动作历史学流匹配。运行只单次视觉编码，动作仍去噪10或16步，输出32动作并执行指定前缀。

## 技术挂点

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。

- [教师学生蒸馏](../concepts/distill.md)：用教师的预测分布、特征或动作监督学生，把已有模型的可用信息迁移到学生。

- [视频时序生成](../concepts/video.md)：同时表达画面内容与时间变化，用历史与条件产生连续帧。

- [Flow Matching](../concepts/flow.md)：给噪声到数据指定概率路径，回归沿路径的速度场；生成时数值积分这个场。

- [Diffusion Transformer](../concepts/dit.md)：用 Transformer 实现扩散模型的去噪网络，使 token 之间交换条件与目标信息。

- [变分自编码器 VAE](../concepts/vae.md)：编码器描述潜变量分布，解码器从潜变量重建样本，用重建与分布正则共同训练。

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。

- [动作块](../concepts/chunk.md)：一次预测多个未来控制时刻的动作，再执行部分并用新观测更新。

- [机器人数据与评测](../concepts/data.md)：统一观测、动作、任务与评测条件，判断数据多样性如何影响泛化。

- [跨本体数据](../concepts/cross-body.md)：从多个机器人或人类收集经验，通过动作/观测适配接到共享学习系统。

- [泛化评测与遗忘](../concepts/benchmark.md)：拆开任务、物体、场景或学习顺序，检查迁移能力和旧技能保留。

## 本篇行星与卫星

- [表征空间](dreamfree/representation.md) · 初读挂点
- [教师学生蒸馏](dreamfree/distill.md) · 初读挂点
- [视频时序生成](dreamfree/video.md) · 初读挂点
- [Flow Matching](dreamfree/flow.md) · 初读挂点
- [Diffusion Transformer](dreamfree/dit.md) · 初读挂点
- [变分自编码器 VAE](dreamfree/vae.md) · 初读挂点
- [注意力](dreamfree/attention.md) · 初读挂点
- [动作块](dreamfree/chunk.md) · 初读挂点
- [机器人数据与评测](dreamfree/data.md) · 初读挂点
- [跨本体数据](dreamfree/cross-body.md) · 初读挂点
- [泛化评测与遗忘](dreamfree/benchmark.md) · 初读挂点
- [本篇方法链路](dreamfree/method-chain.md) · 初读挂点
- [生成未来视频是否是控制必需](dreamfree/df-problem.md) · 初读挂点
- [机器人视频域适配](dreamfree/df-adapt.md) · 初读挂点
- [当前帧可见性约束](dreamfree/df-mask.md) · 初读挂点
- [冻结的未来表征教师](dreamfree/df-teacher.md) · 初读挂点
- [教师固定噪声水平](dreamfree/df-noise.md) · 初读挂点
- [从当前token扩展未来token](dreamfree/df-projector.md) · 初读挂点
- [未来token余弦蒸馏](dreamfree/df-distill.md) · 初读挂点
- [生成流匹配正则](dreamfree/df-gen.md) · 初读挂点
- [冻结编码器再学动作](dreamfree/df-stage2.md) · 初读挂点
- [64个可学习动作查询](dreamfree/df-readout.md) · 初读挂点
- [1B动作DiT流匹配](dreamfree/df-action.md) · 初读挂点
- [DROID八步动作历史](dreamfree/df-history.md) · 初读挂点
- [32步预测与执行窗口](dreamfree/df-execution.md) · 初读挂点
- [冻结特征的动作与未来探针](dreamfree/df-probes.md) · 初读挂点
- [LIBERO四套任务](dreamfree/df-libero.md) · 初读挂点
- [RoboCasa厨房任务](dreamfree/df-robocasa.md) · 初读挂点
- [蒸馏与生成目标消融](dreamfree/df-ablation.md) · 初读挂点
- [骨干规模与额外视频](dreamfree/df-scaling.md) · 初读挂点
- [DROID五十次实机比较](dreamfree/df-droid.md) · 初读挂点
- [成功率与进度分分开](dreamfree/df-progress.md) · 初读挂点
- [双臂YAM定性执行](dreamfree/df-yam.md) · 初读挂点
- [H200单chunk计算成本](dreamfree/df-latency.md) · 初读挂点
- [积木任务完成时间估计](dreamfree/df-completion.md) · 初读挂点
- [视频可教任务组合](dreamfree/df-transfer.md) · 初读挂点
- [跨本体视频任务迁移](dreamfree/df-cross.md) · 初读挂点
- [十段视频后适配](dreamfree/df-adaptation.md) · 初读挂点
- [原子动作缺口仍会阻断迁移](dreamfree/df-failures.md) · 初读挂点
- [训练成本与代码状态](dreamfree/df-compute.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
