# 3.1 统一动作编码：208究竟怎么算出来的？ · Holo-M

先拆 B。一次输出一秒动作，采样 30 Hz，等于 30 个时刻。用 A<sub>t</sub> 表示从时刻 t 开始的动作块；“∥”把四组沿列拼接，“∈”表示属于，ℝ 是实数集合。于是 A<sub>t</sub> 是 30×96 的实数矩阵。<!-- evidence:C04 -->

先拆 B。一次输出一秒动作，采样 30 Hz，等于 30 个时刻。用 A<sub>t</sub> 表示从时刻 t 开始的动作块；“∥”把四组沿列拼接，“∈”表示属于，ℝ 是实数集合。于是 A<sub>t</sub> 是 30×96 的实数矩阵。 动作矩阵：行是时间，列是四组动作表示（原文 Eq. 1–3）。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/holo-m-2609.35709/README.md#31-统一动作编码208究竟怎么算出来的)

[本篇星系](../holo-m.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/holo-m-2609.35709/README.md) · [原文依据](https://arxiv.org/abs/2609.35709)
