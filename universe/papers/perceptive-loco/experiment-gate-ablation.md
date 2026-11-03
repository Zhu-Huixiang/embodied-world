# 用四种编码器分开检验记忆与门控 · Perceptive Locomotion

消融比较GRU或MLP、带门或不带门，查看模仿、重建、奖励与过阶。

它比纯本体控制器对比更接近门控贡献问题；训练曲线也受到逐步加大噪声和地形课程影响。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#410-附录消融门控到底帮在哪里)

继续拆：[门控动作误差优势要逐条件读](experiment-action-error.md) · [重建更准与行走成功分开验证](experiment-reconstruction-error.md) · [每高度100次的仿真过阶消融](experiment-step-ablation.md)。

[本篇星系](../perceptive-loco.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md) · [原文依据](https://leggedrobotics.github.io/rl-perceptiveloco/assets/pdf/wild_anymal.pdf)
