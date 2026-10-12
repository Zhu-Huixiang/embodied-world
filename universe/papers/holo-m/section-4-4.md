# 4.4 数据消融：A区那批人的手，帮了多少忙？ · Holo-M

Table 5 固定 AR 骨干与动作组顺序，换动作预训练数据。所有设置都从预训练 VLM 出发，“无”指跳过动作数据预训练。<!-- evidence:C07 -->

Table 5 固定 AR 骨干与动作组顺序，换动作预训练数据。所有设置都从预训练 VLM 出发，“无”指跳过动作数据预训练。 先加人形数据，多成功 66 次；再加人类 EgoDex，多 19 次。回看 A→B→E，那条只提供 EEF 的支路确实帮上了忙。接下来固定数据量，拿掉 EEF 共享组或换 tokenizer，看看哪项任务先掉：能把“多看了动作”与“共享表示好用”进一步拆开。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/holo-m-2609.35709/README.md#44-数据消融a区那批人的手帮了多少忙)

[本篇星系](../holo-m.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/holo-m-2609.35709/README.md) · [原文依据](https://arxiv.org/abs/2609.35709)
