# 密集掩码提示 · SAM

粗掩码保留空间排列并加到图像特征。

256²掩码经步幅卷积变成64²×256；无掩码使用可学习缺省嵌入。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam-2304.02643/README.md#32-b-区提示也得翻译成模型能计算的对象)

[本篇星系](../sam.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam-2304.02643/README.md) · [原文依据](https://arxiv.org/abs/2304.02643v1)
