# La-JEPA 星系

La-JEPA: Compact Robot Policies with Latent World Modeling

**导读** · 世界动作模型

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/la-jepa.md) · [原文](https://arxiv.org/abs/2611.08156v1) · [评分卡](../../leaderboard/papers/la-jepa/README.md)

La-JEPA以预训练V-JEPA 2.1 ViT-L编码当前两帧和32帧范围内的未来16帧，FLAN-T5-large编码语言，本体投影为条件token。在该表征空间从头训练World DiT和Action DiT，分别对未来特征与32步动作块做独立时间的流匹配。观测只读观测、未来读观测和未来、动作只读观测和动作；未来损失通过共享World参数影响观测表示。部署删除未来token，固定World时间0并缓存观测K/V，仅对动作做10步Euler积分，LIBERO执行10步、RoboTwin执行24步后重规划。最终观测编码器用LoRA和增强，未来目标保持原冻结编码器的干净特征；无需像素解码。

## 技术挂点

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。

- [表征预测 JEPA](../concepts/jepa.md)：在表征空间预测目标而不是逐像素重建；防止表征坍缩仍需要相应设计。

- [世界模型](../concepts/world.md)：学习状态随动作或时间如何变化，用于预测、计划或训练策略。

- [世界动作联合建模](../concepts/wam.md)：把未来状态或视频与动作放进联合条件生成过程，让视觉动态和行动相互约束。

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。

- [因果序列建模](../concepts/causal.md)：通过遮罩只让位置读取允许的历史，避免训练时看到运行时不存在的未来。

- [Flow Matching](../concepts/flow.md)：给噪声到数据指定概率路径，回归沿路径的速度场；生成时数值积分这个场。

- [Diffusion Transformer](../concepts/dit.md)：用 Transformer 实现扩散模型的去噪网络，使 token 之间交换条件与目标信息。

- [动作块](../concepts/chunk.md)：一次预测多个未来控制时刻的动作，再执行部分并用新观测更新。

- [示范模仿](../concepts/imitation.md)：从专家、人类或教师策略的行为学习动作，研究数据、表示和执行误差。

- [分布偏移](../concepts/shift.md)：测试场景的画风、视角、背景或对象组合发生变化，模型习惯的视觉线索随之改变。

- [机器人数据与评测](../concepts/data.md)：统一观测、动作、任务与评测条件，判断数据多样性如何影响泛化。

- [泛化评测与遗忘](../concepts/benchmark.md)：拆开任务、物体、场景或学习顺序，检查迁移能力和旧技能保留。

## 本篇行星与卫星

- [表征空间](la-jepa/representation.md) · 初读挂点
- [表征预测 JEPA](la-jepa/jepa.md) · 初读挂点
- [世界模型](la-jepa/world.md) · 初读挂点
- [世界动作联合建模](la-jepa/wam.md) · 初读挂点
- [注意力](la-jepa/attention.md) · 初读挂点
- [因果序列建模](la-jepa/causal.md) · 初读挂点
- [Flow Matching](la-jepa/flow.md) · 初读挂点
- [Diffusion Transformer](la-jepa/dit.md) · 初读挂点
- [动作块](la-jepa/chunk.md) · 初读挂点
- [示范模仿](la-jepa/imitation.md) · 初读挂点
- [分布偏移](la-jepa/shift.md) · 初读挂点
- [机器人数据与评测](la-jepa/data.md) · 初读挂点
- [泛化评测与遗忘](la-jepa/benchmark.md) · 初读挂点
- [本篇方法链路](la-jepa/method-chain.md) · 初读挂点
- [机器人策略一定要继承大生成骨干吗](la-jepa/la-jepa-problem.md) · 初读挂点
- [多相机、本体与指令各走哪条路](la-jepa/la-jepa-input.md) · 初读挂点
- [当前两帧与未来十六帧分开编码](la-jepa/la-jepa-tube.md) · 初读挂点
- [平均与拼接都减少token，但保留信息不同](la-jepa/la-jepa-spatial.md) · 初读挂点
- [动作看观测，不直接看未来token](la-jepa/la-jepa-mask.md) · 初读挂点
- [两个独立流时间，两个速度目标](la-jepa/la-jepa-flow.md) · 初读挂点
- [部署删未来，再缓存观测键值](la-jepa/la-jepa-inference.md) · 初读挂点
- [0.10B可训练不等于0.10B部署](la-jepa/la-jepa-size.md) · 初读挂点
- [未来监督的收益要在同一管线内看](la-jepa/la-jepa-future-ablation.md) · 初读挂点
- [JEPA与VAE比的是表征系统](la-jepa/la-jepa-feature-space.md) · 初读挂点
- [防止策略只抄本体或依赖一个相机](la-jepa/la-jepa-robustness.md) · 初读挂点
- [适配观测并不要求目标也随之漂移](la-jepa/la-jepa-targets.md) · 初读挂点
- [数据回放成功和关节连续性先过关](la-jepa/la-jepa-data.md) · 初读挂点
- [同一指令协议下比较小模型](la-jepa/la-jepa-libero.md) · 初读挂点
- [视觉扰动标签不该混进动作指令](la-jepa/la-jepa-instruction.md) · 初读挂点
- [clean学到的技能在随机场景剩多少](la-jepa/la-jepa-robotwin.md) · 初读挂点
- [20任务与50任务不能无条件互换](la-jepa/la-jepa-latent-comparison.md) · 初读挂点
- [一次策略调用快，不等于机器人控制频率](la-jepa/la-jepa-latency.md) · 初读挂点
- [CUDA图可逐位一致，编译版本另做闭环核对](la-jepa/la-jepa-compile.md) · 初读挂点
- [四项桌面任务检验接触与长链](la-jepa/la-jepa-real.md) · 初读挂点
- [摆上盘子不是整条餐具任务完成](la-jepa/la-jepa-dish.md) · 初读挂点
- [大模型未单调更好，广泛预训练仍待验证](la-jepa/la-jepa-limits.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
