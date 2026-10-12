# 本篇方法链路 · Octo

各类任务、图像和本体感觉先由模态 tokenizer 转成 token，Transformer 主干处理后由读取头和扩散解码器产生动作块。更换机器人时，输入或输出适配器可改变，而主干保留预训练知识并微调。项目在不同平台上区分零样本运行与小数据微调，还单独检验新力传感输入和关节控制空间。

各类任务、图像和本体感觉先由模态 tokenizer 转成 token，Transformer 主干处理后由读取头和扩散解码器产生动作块。更换机器人时，输入或输出适配器可改变，而主干保留预训练知识并微调。项目在不同平台上区分零样本运行与小数据微调，还单独检验新力传感输入和关节控制空间。

[本篇星系](../octo.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/octo.md) · [原文依据](https://www.roboticsproceedings.org/rss20/p090.html)
