# 本篇方法链路 · JEDI

每段示范由4层Perceiver独立压成8个slot并缓存；π0的flow-matching动作专家读取查询观测与这些slot。辅助预测器在冻结V-JEPA2.1空间预测查询回合下一关键帧，对当前观测支路stop-gradient，使预测损失真正训练示范压缩器。错误任务和同任务不同过程的反事实margin约束保留目标/顺序。用示范间交叉预测误差和查询初图相似性选取一致示范，支持阶段性commitment；人类视频扩展经同平台真实posttraining，用手/物体关键点补充对应，不是任意人类视频免训练通用控制。

每段示范由4层Perceiver独立压成8个slot并缓存；π0的flow-matching动作专家读取查询观测与这些slot。辅助预测器在冻结V-JEPA2.1空间预测查询回合下一关键帧，对当前观测支路stop-gradient，使预测损失真正训练示范压缩器。错误任务和同任务不同过程的反事实margin约束保留目标/顺序。用示范间交叉预测误差和查询初图相似性选取一致示范，支持阶段性commitment；人类视频扩展经同平台真实posttraining，用手/物体关键点补充对应，不是任意人类视频免训练通用控制。

[本篇星系](../jedi.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/jedi.md) · [原文依据](https://arxiv.org/abs/2610.40356v1)
