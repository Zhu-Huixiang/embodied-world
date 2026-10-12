# 本篇方法链路 · VIMA

对象图像 token 与文字交错构成任务提示，再经 T5 编码；因果 Transformer 通过交叉注意力读取提示，并结合交互历史自回归输出动作。程序化生成任务按不同泛化难度拆开测试，避免只看训练分布平均成功率。原文对对象 tokenizer、提示接入方式、模型规模和数据量分别消融。

对象图像 token 与文字交错构成任务提示，再经 T5 编码；因果 Transformer 通过交叉注意力读取提示，并结合交互历史自回归输出动作。程序化生成任务按不同泛化难度拆开测试，避免只看训练分布平均成功率。原文对对象 tokenizer、提示接入方式、模型规模和数据量分别消融。

[本篇星系](../vima.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/vima.md) · [原文依据](https://proceedings.mlr.press/v202/jiang23b.html)
