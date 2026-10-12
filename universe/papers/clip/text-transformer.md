# 文本 Transformer · CLIP

文本token通过因果注意力读取前文。

B/32版文本网络宽512、12层、8头；最终取EOS位置特征再投影。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#23-模型两边各自干活最后才对答案)

继续拆：[BPE 与字节分词](bpe.md) · [EOS 与因果注意力](eos.md)。

[本篇星系](../clip.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md) · [原文依据](https://proceedings.mlr.press/v139/radford21a.html)
