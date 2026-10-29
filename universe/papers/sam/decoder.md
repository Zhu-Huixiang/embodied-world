# 双向注意力解码 · SAM

token读图像后，图像再读token。

两层内按token自注意力、token到图像、MLP、图像到token更新两路状态。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam-2304.02643/README.md#33-c-区提示看图图也回头看提示)

继续拆：[交叉注意力的两种方向](cross.md) · [掩码超网络读出](readout.md)。

[本篇星系](../sam.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam-2304.02643/README.md) · [原文依据](https://arxiv.org/abs/2304.02643v1)
