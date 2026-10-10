# Attention Is All You Need

出处：NeurIPS 2017。研究范围：生成/表征基础，VLA、动作 Transformer 与视频模型共用的注意力计算。

[原文入口](https://papers.nips.cc/paper/2017/hash/3f5ee243547dee91fbd053c1c4a845aa-Abstract.html) · [原文 PDF](https://papers.neurips.cc/paper_files/paper/2017/file/3f5ee243547dee91fbd053c1c4a845aa-Paper.pdf) · [作者项目 / 代码入口](https://github.com/tensorflow/tensor2tensor)

正式出处为 NIPS 2017（现名 NeurIPS）；保留原始会议论文，机器翻译实验与后续机器人应用分开。

阅读问题：**Q、K、V 到底在计算什么，为什么这套序列计算能连接视觉、语言和动作？**

收录理由：多头自注意力、位置编码及因果遮罩是后续 VLA/ACT/DiT 的直接计算基础，用户明确点名允许此类经典例外。

证据入口：纯注意力替代循环网络的计算改动清晰，翻译对照和结构消融完整，官方实现公开；具身价值来自下游共享结构。

具身关联：多头自注意力、位置编码及因果遮罩是后续 VLA/ACT/DiT 的直接计算基础，用户明确点名允许此类经典例外。

经典保留理由：2017 年经典例外：用户明确举例允许；Transformer 的 Q/K/V、多头注意力和因果建模是现代具身视觉语言动作模型的共同基础。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/attention/README.md)

机制简析：输入 token 先做词嵌入和位置编码，再由多头注意力计算每个位置该从哪些位置取信息。编码器使用全序列自注意力；解码器用因果遮罩阻止读取未来 token，并通过交叉注意力接收编码器输出。原文在两项 WMT 翻译任务比较质量、训练成本与不同注意力配置。
<!-- discovery:end -->
