# CR-DAgger 星系

Compliant Residual DAgger: Improving Real-World Contact-Rich Manipulation with Human Corrections

**导读** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/cr-dagger.md) · [原文](https://proceedings.nips.cc/paper_files/paper/2025/hash/cbf883a744952d4a40591271a58ab9d0-Abstract-Conference.html) · [评分卡](../../leaderboard/papers/cr-dagger/README.md)

CR-DAgger保留低频扩散基策略，通过顺应式动觉接口在策略继续运行时采集人的位置增量和接触力纠正。扩展稿用参考速度跟踪和硬件时延对齐避免微小纠正标签被控制滞后淹没。冻结视觉编码器，力历史经时间卷积，与状态共同输入轻量残差头；残差推理循环约50Hz，每次预测5个间隔0.02s的15维动作（9维位姿表示与6维目标力/力矩），由500Hz导纳控制器执行基准动作加局部修正。无干预段学零残差，并对纠正附近数据重采样，避免用少量新数据直接改坏完整基策略。

## 技术挂点

- [示范模仿](../concepts/imitation.md)：从专家、人类或教师策略的行为学习动作，研究数据、表示和执行误差。

- [行为克隆](../concepts/bc.md)：直接监督观测到动作的映射，不必在每次更新中根据奖励搜索。

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。

- [动作块](../concepts/chunk.md)：一次预测多个未来控制时刻的动作，再执行部分并用新观测更新。

- [扩散去噪](../concepts/diffusion.md)：训练网络从带噪对象估计噪声或干净目标，生成时从噪声开始迭代恢复样本。

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。

- [机器人数据与评测](../concepts/data.md)：统一观测、动作、任务与评测条件，判断数据多样性如何影响泛化。

- [泛化评测与遗忘](../concepts/benchmark.md)：拆开任务、物体、场景或学习顺序，检查迁移能力和旧技能保留。

## 本篇行星与卫星

- [示范模仿](cr-dagger/imitation.md) · 初读挂点
- [行为克隆](cr-dagger/bc.md) · 初读挂点
- [动作表示](cr-dagger/action.md) · 初读挂点
- [动作块](cr-dagger/chunk.md) · 初读挂点
- [扩散去噪](cr-dagger/diffusion.md) · 初读挂点
- [表征空间](cr-dagger/representation.md) · 初读挂点
- [机器人数据与评测](cr-dagger/data.md) · 初读挂点
- [泛化评测与遗忘](cr-dagger/benchmark.md) · 初读挂点
- [本篇方法链路](cr-dagger/method-chain.md) · 初读挂点
- [接触纠错为何难以喂回策略](cr-dagger/cr-problem.md) · 初读挂点
- [边运行边推一把的顺应接口](cr-dagger/cr-interface.md) · 初读挂点
- [质量弹簧阻尼式导纳控制](cr-dagger/cr-controller.md) · 初读挂点
- [把参考速度放回阻尼项](cr-dagger/cr-tracking.md) · 初读挂点
- [给纠正标签补偿硬件延迟](cr-dagger/cr-latency.md) · 初读挂点
- [On-Policy Delta与接管的区别](cr-dagger/cr-onpolicy.md) · 初读挂点
- [冻结低频扩散基策略](cr-dagger/cr-base.md) · 初读挂点
- [约50Hz推理的力感知残差策略](cr-dagger/cr-residual.md) · 初读挂点
- [时间卷积读取接触力历史](cr-dagger/cr-force-encoder.md) · 初读挂点
- [15维动作与目标力/力矩](cr-dagger/cr-action.md) · 初读挂点
- [500Hz控制闭环接住两种动作](cr-dagger/cr-execution.md) · 初读挂点
- [无干预时也教残差归零](cr-dagger/cr-label.md) · 初读挂点
- [多采纠正后的接触片段](cr-dagger/cr-sampling.md) · 初读挂点
- [少量多轮更新未必更好](cr-dagger/cr-batches.md) · 初读挂点
- [翻书：看纠正方式与力是否都需要](cr-dagger/cr-book.md) · 初读挂点
- [皮带装配：同任务比较力与更新方式](cr-dagger/cr-belt.md) · 初读挂点
- [齿轮插入：亚毫米接触纠正](cr-dagger/cr-gear.md) · 初读挂点
- [布线：线材和夹具的物理变化](cr-dagger/cr-cable.md) · 初读挂点
- [阶段成功率定位失败点](cr-dagger/cr-stage.md) · 初读挂点
- [残差头结构不是唯一解释](cr-dagger/cr-architecture.md) · 初读挂点
- [人类纠正与硬件成本](cr-dagger/cr-cost.md) · 初读挂点
- [四项真实任务的证据边界](cr-dagger/cr-scope.md) · 初读挂点
- [原会议稿与期刊扩展稿同一研究](cr-dagger/cr-edition.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
