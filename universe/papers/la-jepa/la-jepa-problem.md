# 机器人策略一定要继承大生成骨干吗 · La-JEPA

感知预训练的价值与生成骨干的体量可以分开选择。

论文把问题落在仅使用目标示范的操控：保留预训练视觉/语言编码器，从头训练面向控制的World/Action DiT，而不是把视频生成器整个搬来。

继续拆：[多相机、本体与指令各走哪条路](la-jepa-input.md) · [数据回放成功和关节连续性先过关](la-jepa-data.md) · [四项桌面任务检验接触与长链](la-jepa-real.md) · [大模型未单调更好，广泛预训练仍待验证](la-jepa-limits.md)。

[本篇星系](../la-jepa.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/la-jepa.md) · [原文依据](https://arxiv.org/pdf/2611.08156v1)
