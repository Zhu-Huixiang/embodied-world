# 双编码器 · CLIP

图和文字分别计算，再比较最终向量。

视觉和文本网络没有逐图块逐单词联合重算；这让类别文字可以预先缓存。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#23-模型两边各自干活最后才对答案)

继续拆：[视觉 Transformer](vit.md) · [文本 Transformer](text-transformer.md) · [LayerNorm](layernorm.md) · [线性投影与共同空间](projection.md)。

[本篇星系](../clip.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md) · [原文依据](https://proceedings.mlr.press/v139/radford21a.html)
