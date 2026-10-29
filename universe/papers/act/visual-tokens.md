# 视觉token形状 · ACT / ALOHA

四路ResNet特征拼成1200×512序列。

15×20空间展平为每相机300token，再加关节与z两个token。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/act-2304.13705/README.md#44-transformer四台相机怎样变成10014)

继续拆：[观察序列融合](observation-fusion.md)。

[本篇星系](../act.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/act-2304.13705/README.md) · [原文依据](https://www.roboticsproceedings.org/rss19/p016.html)
