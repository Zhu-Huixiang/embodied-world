# 视觉 Transformer · CLIP

图像切块并经过注意力网络，汇成图像特征。

B/32把224×224图像切成49个32×32图块，加CLS后共有50个视觉token；每个宽768。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#23-模型两边各自干活最后才对答案)

继续拆：[CLS 汇总 token](cls.md)。

[本篇星系](../clip.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md) · [原文依据](https://proceedings.mlr.press/v139/radford21a.html)
