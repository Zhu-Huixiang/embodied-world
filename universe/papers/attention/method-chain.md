# 本篇方法链路 · Transformer

输入 token 先做词嵌入和位置编码，再由多头注意力计算每个位置该从哪些位置取信息。编码器使用全序列自注意力；解码器用因果遮罩阻止读取未来 token，并通过交叉注意力接收编码器输出。原文在两项 WMT 翻译任务比较质量、训练成本与不同注意力配置。

输入 token 先做词嵌入和位置编码，再由多头注意力计算每个位置该从哪些位置取信息。编码器使用全序列自注意力；解码器用因果遮罩阻止读取未来 token，并通过交叉注意力接收编码器输出。原文在两项 WMT 翻译任务比较质量、训练成本与不同注意力配置。

[本篇星系](../attention.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/attention.md) · [原文依据](https://papers.nips.cc/paper/2017/hash/3f5ee243547dee91fbd053c1c4a845aa-Abstract.html)
