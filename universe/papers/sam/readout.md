# 掩码超网络读出 · SAM

输出token生成32维逐像素读出权重。

上采样得到256²×32特征，与各mask token生成的向量点积得到候选logit。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam-2304.02643/README.md#33-c-区提示看图图也回头看提示)

[本篇星系](../sam.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/sam-2304.02643/README.md) · [原文依据](https://arxiv.org/abs/2304.02643v1)
