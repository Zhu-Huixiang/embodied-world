# 4.5 实机部署：F区，时钟开始较真了 · Holo-M

实机是 G1-comp、两只 Dex3 手、头部 RealSense 相机，单张 RTX 5090 推理。RGB 图像 640×360，相机 30 Hz；策略每 500 ms 取一份观测。输入关节状态是 31 个上半身角度：14 手部、14 手臂、腰部三个转角，每个角度选一个 256 档状态 token。下肢状态交给控制栈，策略按画面、这些角度与任务指令预测一秒动作。<!-- evidence:C15 -->

实机是 G1-comp、两只 Dex3 手、头部 RealSense 相机，单张 RTX 5090 推理。RGB 图像 640×360，相机 30 Hz；策略每 500 ms 取一份观测。输入关节状态是 31 个上半身角度：14 手部、14 手臂、腰部三个转角，每个角度选一个 256 档状态 token。下肢状态交给控制栈，策略按画面、这些角度与任务指令预测一秒动作。 第三个问题要在 F 答完：组内并行减少生成轮次，旧动作块与新推理交叠，身体才一直有目标可执行。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/holo-m-2609.35709/README.md#45-实机部署f区时钟开始较真了)

[本篇星系](../holo-m.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/holo-m-2609.35709/README.md) · [原文依据](https://arxiv.org/abs/2609.35709)
