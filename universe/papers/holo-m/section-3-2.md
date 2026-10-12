# 3.2 VLM 骨干：C区到底往模型里塞了什么？ · Holo-M

动作有写法了，模型还得知道眼前发生了啥。C 区把输入按图像→任务→setup→状态排列：图像回答“在哪儿”，任务回答“做什么”，setup 标识本体与数据来源，状态报当前关节位置。图像走视觉编码器，剩下的变成离散 token，然后一起进 D 区的 Qwen3-VL-2B。<!-- evidence:C22 -->

动作有写法了，模型还得知道眼前发生了啥。C 区把输入按图像→任务→setup→状态排列：图像回答“在哪儿”，任务回答“做什么”，setup 标识本体与数据来源，状态报当前关节位置。图像走视觉编码器，剩下的变成离散 token，然后一起进 D 区的 Qwen3-VL-2B。 条件序列与自回归分解：先前组、当前组先前 token 都进入条件（原文 Eq. 9–10）。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/holo-m-2609.35709/README.md#32-vlm-骨干c区到底往模型里塞了什么)

[本篇星系](../holo-m.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/holo-m-2609.35709/README.md) · [原文依据](https://arxiv.org/abs/2609.35709)
