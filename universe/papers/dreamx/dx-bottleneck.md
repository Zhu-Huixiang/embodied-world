# 32乘2048再压成32乘32 · DreamX

token少了，通道仍大；单独变分瓶颈进一步压通道。

单自注意力编码器输出32维高斯code，六层Transformer解码2048维特征；重建+0.01KL，5万步，训练后取posterior mean。

继续拆：[控制时预测code而非生成未来视频](dx-policy.md)。

[本篇星系](../dreamx.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamx.md) · [原文依据](https://arxiv.org/pdf/2611.05377v1)
