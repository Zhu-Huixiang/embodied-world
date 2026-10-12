# CLIP 星系

Learning Transferable Visual Models From Natural Language Supervision

**已精讲** · 具身感知与场景表示

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md) · [原文](https://proceedings.mlr.press/v139/radford21a.html) · [评分卡](../../leaderboard/papers/clip/README.md)

图像编码器和文本编码器分别输出向量，经投影与归一化后计算一个批次中全部图文配对的相似度矩阵。对称交叉熵把真实配对拉近，把批内错配分开；测试时用文本描述生成类别向量，从而做零样本分类。原文在三十余个视觉数据集测试迁移，CLIPort 再将其语义特征与空间操作分支融合。

## 技术挂点

- [对比学习](../concepts/contrastive.md)：给相关样本较高相似度，让它们在候选竞争中被找回来。图文配对是 CLIP 的监督来源。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#22-训练目标完整写一句话负担有点重)

- [向量归一化](../concepts/normalization.md)：把向量除以自己的 L2 长度，得到单位向量。点积随后比较方向，减少向量大小的干扰。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#22-训练目标完整写一句话负担有点重)

- [余弦相似度](../concepts/cosine.md)：两个向量点积再除以各自长度。单位向量的点积直接等于余弦相似度。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#22-训练目标完整写一句话负担有点重)

- [交叉熵](../concepts/cross-entropy.md)：正确候选的负对数概率。正确项概率越小，损失越大，梯度会推动正确分数上升。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#22-训练目标完整写一句话负担有点重)

- [softmax 与温度](../concepts/softmax.md)：对候选分数取指数后归一化为总和为 1 的概率。温度控制分差如何影响概率。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#22-训练目标完整写一句话负担有点重)

- [视觉 patch token](../concepts/patches.md)：把图像切成块，展平并投影成向量，再加入位置信息。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#23-模型两边各自干活最后才对答案)

- [零样本任务接口](../concepts/zero-shot.md)：不用目标数据集训练样本拟合分类头，而用任务描述等已有信息直接构造预测接口。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#25-使用一句话怎样变成分类器)

- [提示模板集成](../concepts/prompt-ensemble.md)：同一类别放进多种句子模板，编码后平均并归一化，减少单一表述对分类权重的影响。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#25-使用一句话怎样变成分类器)

- [线性探测](../concepts/linear-probe.md)：冻结编码器，用带标签的下游样本训练线性预测头，以检查特征本身是否容易迁移。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#33-表征换个分类头才能单独看视觉底子)

- [分布偏移](../concepts/shift.md)：测试场景的画风、视角、背景或对象组合发生变化，模型习惯的视觉线索随之改变。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#34-换场景香蕉一变成素描就不认识了)

- [空间表示](../concepts/spatial.md)：保留像素、点、体素或对象相对位置的表示，让预测能接到几何与动作位置。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/clip-2103.00020/README.md#6-局限认出杯子距离抓住杯子还差什么)

## 本篇行星与卫星

- [对比学习](clip/contrastive.md) · 已讲解
- [向量归一化](clip/normalization.md) · 已讲解
- [余弦相似度](clip/cosine.md) · 已讲解
- [交叉熵](clip/cross-entropy.md) · 已讲解
- [softmax 与温度](clip/softmax.md) · 已讲解
- [视觉 patch token](clip/patches.md) · 已讲解
- [零样本任务接口](clip/zero-shot.md) · 已讲解
- [提示模板集成](clip/prompt-ensemble.md) · 已讲解
- [线性探测](clip/linear-probe.md) · 已讲解
- [分布偏移](clip/shift.md) · 已讲解
- [空间表示](clip/spatial.md) · 已讲解
- [本篇方法链路](clip/method-chain.md) · 已讲解
- [图文数据与监督](clip/data.md) · 已讲解
- [配文噪声与局部监督](clip/noise.md) · 已讲解
- [检索覆盖与数据配额](clip/query-balance.md) · 已讲解
- [双编码器](clip/dual-encoder.md) · 已讲解
- [视觉 Transformer](clip/vit.md) · 已讲解
- [CLS 汇总 token](clip/cls.md) · 已讲解
- [文本 Transformer](clip/text-transformer.md) · 已讲解
- [BPE 与字节分词](clip/bpe.md) · 已讲解
- [EOS 与因果注意力](clip/eos.md) · 已讲解
- [LayerNorm](clip/layernorm.md) · 已讲解
- [线性投影与共同空间](clip/projection.md) · 已讲解
- [批内相似度矩阵](clip/pair-matrix.md) · 已讲解
- [正配对、负例与假负例](clip/positive-negative.md) · 已讲解
- [双向交叉熵](clip/bidirectional.md) · 已讲解
- [梯度如何推动配对](clip/gradient.md) · 已讲解
- [温度与可学习缩放](clip/temperature.md) · 已讲解
- [大批次与训练规模](clip/batch-scale.md) · 已讲解
- [生成配文与配对判别](clip/caption-vs-contrast.md) · 已讲解
- [文本生成类别权重](clip/class-weights.md) · 已讲解
- [类别向量缓存](clip/cache.md) · 已讲解
- [提示上下文与歧义](clip/ambiguity.md) · 已讲解
- [候选集合与拒识](clip/closed-set.md) · 已讲解
- [少样本线性分类](clip/few-shot.md) · 已讲解
- [推理计算与迁移得分](clip/compute-transfer.md) · 已讲解
- [视频任务的单帧评估](clip/video-frame.md) · 已讲解
- [自然分布偏移与有效鲁棒性](clip/robustness.md) · 已讲解
- [bootstrap 置信区间](clip/bootstrap.md) · 已讲解
- [目标分布适配的代价](clip/adaptation-tradeoff.md) · 已讲解
- [近重复检测与语义相似](clip/dedup.md) · 已讲解
- [类别设计与社会偏差](clip/bias.md) · 已讲解
- [CLIPort 的 what / where](clip/cliport.md) · 已讲解
- [语义与控制的接口差距](clip/spatial-action-gap.md) · 已讲解

## 论文间的联系

- [CLIPort](cliport.md) → [CLIP](clip.md)：CLIPort 冻结 CLIP 提供语义特征，融合保留空间结构的分支。 [原文定位](https://proceedings.mlr.press/v164/shridhar22a.html)（CLIPort §4.2 semantic stream; CLIP article §8, evidence C21）。

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
