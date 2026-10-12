# 3.3 分组离散扩散：D区从打字改成填空 · Holo-M

Holo-M 把当前组改成“大家一起猜”。训练先挖一些空，模型看着可见位置和前面的组，把空补回来。用 p<sub>g</sub> 表示随机遮盖概率，M<sub>g</sub> 是本次被遮住的有效位置集合，N<sub>g</sub> 是该组有效 token 数。这里 N<sub>g</sub> 数 token，上一节 N=2 数低频系数，别串台。<!-- evidence:C20 -->

Holo-M 把当前组改成“大家一起猜”。训练先挖一些空，模型看着可见位置和前面的组，把空补回来。用 p<sub>g</sub> 表示随机遮盖概率，M<sub>g</sub> 是本次被遮住的有效位置集合，N<sub>g</sub> 是该组有效 token 数。这里 N<sub>g</sub> 数 token，上一节 N=2 数低频系数，别串台。 当前组的恢复目标：只对被 mask 的有效位置计算交叉熵（原文 Eq. 11–12）。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/holo-m-2609.35709/README.md#33-分组离散扩散d区从打字改成填空)

[本篇星系](../holo-m.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/holo-m-2609.35709/README.md) · [原文依据](https://arxiv.org/abs/2609.35709)
