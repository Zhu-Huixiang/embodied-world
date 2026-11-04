# 本篇方法链路 · ∇Mimic

在4096个64步窗口中沿MuJoCo接触动力学求导，逐反向时间步对每个样本的动作cotangent按批中位范数裁剪，再以固定弧度RMS步长构造目标动作、做8次小批回归。G1专用NablaEngine用每world一个warp及整控制步adjoint megakernel降低求导成本。保留TDλ critic、参考姿态残差和回放起点；训练导数在近自接触、近平行胶囊及饱和actuator处采用特定规则，并非处处无偏的精确梯度。

在4096个64步窗口中沿MuJoCo接触动力学求导，逐反向时间步对每个样本的动作cotangent按批中位范数裁剪，再以固定弧度RMS步长构造目标动作、做8次小批回归。G1专用NablaEngine用每world一个warp及整控制步adjoint megakernel降低求导成本。保留TDλ critic、参考姿态残差和回放起点；训练导数在近自接触、近平行胶囊及饱和actuator处采用特定规则，并非处处无偏的精确梯度。

[本篇星系](../nablamimic.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/nablamimic.md) · [原文依据](https://arxiv.org/abs/2610.41654v1)
