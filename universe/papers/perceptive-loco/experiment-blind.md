# 遮挡传感器后退回接触反应 · Perceptive Locomotion

完全遮挡传感器时，缺地图位置以随机值填入，机器人依靠本体反馈继续过阶。

它先撞到台阶立面才调整，上下阶动作不如有感知时平滑；鲁棒退化保住了行走，并没有保留提前看见地形的能力。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md#24-接触之后内部地形怎样改写)

[本篇星系](../perceptive-loco.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/perceptive-loco-2201.08117/README.md) · [原文依据](https://leggedrobotics.github.io/rl-perceptiveloco/assets/pdf/wild_anymal.pdf)
