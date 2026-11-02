# JEDI 星系

JEDI: Joint-Embedding Demonstration Compression for In-Context Imitation Learning

**导读** · 视觉语言动作模型 VLA

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/jedi.md) · [原文](https://arxiv.org/abs/2610.40356v1) · [评分卡](../../leaderboard/papers/jedi/README.md)

每段示范由4层Perceiver独立压成8个slot并缓存；π0的flow-matching动作专家读取查询观测与这些slot。辅助预测器在冻结V-JEPA2.1空间预测查询回合下一关键帧，对当前观测支路stop-gradient，使预测损失真正训练示范压缩器。错误任务和同任务不同过程的反事实margin约束保留目标/顺序。用示范间交叉预测误差和查询初图相似性选取一致示范，支持阶段性commitment；人类视频扩展经同平台真实posttraining，用手/物体关键点补充对应，不是任意人类视频免训练通用控制。

## 技术挂点

- [表征空间](../concepts/representation.md)：把图像、文字或状态编码成可计算的向量。它像坐标纸：距离与方向是否有用，取决于训练目标。

- [表征预测 JEPA](../concepts/jepa.md)：在表征空间预测目标而不是逐像素重建；防止表征坍缩仍需要相应设计。

- [Transformer](../concepts/transformer.md)：用注意力交换 token 信息，再逐位置加工。token 可以来自字词、图像块、状态或动作。

- [注意力](../concepts/attention.md)：按查询与键的匹配权重汇总值向量，使当前位置读取相关位置的信息。

- [Flow Matching](../concepts/flow.md)：给噪声到数据指定概率路径，回归沿路径的速度场；生成时数值积分这个场。

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。

- [动作块](../concepts/chunk.md)：一次预测多个未来控制时刻的动作，再执行部分并用新观测更新。

- [示范模仿](../concepts/imitation.md)：从专家、人类或教师策略的行为学习动作，研究数据、表示和执行误差。

- [跨本体数据](../concepts/cross-body.md)：从多个机器人或人类收集经验，通过动作/观测适配接到共享学习系统。

- [机器人数据与评测](../concepts/data.md)：统一观测、动作、任务与评测条件，判断数据多样性如何影响泛化。

- [泛化评测与遗忘](../concepts/benchmark.md)：拆开任务、物体、场景或学习顺序，检查迁移能力和旧技能保留。

## 本篇行星与卫星

- [表征空间](jedi/representation.md) · 初读挂点
- [表征预测 JEPA](jedi/jepa.md) · 初读挂点
- [Transformer](jedi/transformer.md) · 初读挂点
- [注意力](jedi/attention.md) · 初读挂点
- [Flow Matching](jedi/flow.md) · 初读挂点
- [动作表示](jedi/action.md) · 初读挂点
- [动作块](jedi/chunk.md) · 初读挂点
- [示范模仿](jedi/imitation.md) · 初读挂点
- [跨本体数据](jedi/cross-body.md) · 初读挂点
- [机器人数据与评测](jedi/data.md) · 初读挂点
- [泛化评测与遗忘](jedi/benchmark.md) · 初读挂点
- [本篇方法链路](jedi/method-chain.md) · 初读挂点
- [示范压缩要保留什么](jedi/jd-compression-question.md) · 初读挂点
- [每条示范独立压成八个slot](jedi/jd-independent-slots.md) · 初读挂点
- [预测查询回合的下一关键帧](jedi/jd-query-future.md) · 初读挂点
- [事件和速度定义关键阶段](jedi/jd-keyframes.md) · 初读挂点
- [阻止观测支路独自消化辅助损失](jedi/jd-stop-gradient.md) · 初读挂点
- [任务与过程反事实负样本](jedi/jd-negatives.md) · 初读挂点
- [过程标签与匹配label对照](jedi/jd-labels.md) · 初读挂点
- [Flow Matching动作专家](jedi/jd-action-expert.md) · 初读挂点
- [示范间预测一致性筛选](jedi/jd-context-selection.md) · 初读挂点
- [阶段完成后保持已选择过程](jedi/jd-commitment.md) · 初读挂点
- [相同动作骨干下的目标消融](jedi/jd-objective-control.md) · 初读挂点
- [自定义未见任务划分](jedi/jd-custom-splits.md) · 初读挂点
- [更多上下文与分布偏移](jedi/jd-many-shot.md) · 初读挂点
- [语言与演示冲突时如何取舍](jedi/jd-language.md) · 初读挂点
- [缓存控制率与bank建立代价](jedi/jd-cost.md) · 初读挂点
- [经过真实posttraining的人类视频接口](jedi/jd-human-transfer.md) · 初读挂点
- [真实任务上的上下文适应](jedi/jd-real-eval.md) · 初读挂点
- [匹配八示范与posttraining控制](jedi/jd-real-matched.md) · 初读挂点
- [单平台、已知动作原语与评价边界](jedi/jd-limits.md) · 初读挂点
- [视觉patch输入与预测目标的维度](jedi/jd-vision-tokens.md) · 初读挂点
- [固定权重下的任务配置适应](jedi/jd-task-context.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
