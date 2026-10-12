# 3.4 四阶段训练：E区让缺标签的数据也能上桌 · Holo-M

第二个问题终于轮到了。人的手部视频怎么参与训练？给每组一个开关 v<sub>g</sub>，标签存在取 1，缺失取 0。EgoDex 只有 EEF，开关就是 (1,0,0,0)。Body、Hand、Kinematics 的损失直接乘零，省掉编假答案。<!-- evidence:C05 -->

第二个问题终于轮到了。人的手部视频怎么参与训练？给每组一个开关 v<sub>g</sub>，标签存在取 1，缺失取 0。EgoDex 只有 EEF，开关就是 (1,0,0,0)。Body、Hand、Kinematics 的损失直接乘零，省掉编假答案。 多来源数据的损失：v<sub>g</sub> 决定哪些组参与，w<sub>g</sub> 决定组间权重（原文 Eq. 13）。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/holo-m-2609.35709/README.md#34-四阶段训练e区让缺标签的数据也能上桌)

[本篇星系](../holo-m.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/holo-m-2609.35709/README.md) · [原文依据](https://arxiv.org/abs/2609.35709)
