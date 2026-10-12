# 向量归一化 · CLIP

把向量除以自己的 L2 长度，得到单位向量。点积随后比较方向，减少向量大小的干扰。

CLIP 两路各投影到共享空间后再归一化；B/32 示例是 N×512。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#22-训练目标完整写一句话负担有点重)

[跨论文技术入口](../../concepts/normalization.md)

[本篇星系](../clip.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md) · [原文依据](https://proceedings.mlr.press/v139/radford21a.html)
