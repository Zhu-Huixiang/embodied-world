# DreamX: Video Diffusion Model is a Universal Latent Action Learner

**解读导读** · arXiv 2026 · [视频动作模型与视觉推理](../paper-map/README.md#track-video-action)

研究范围：跨人/机器人动作表征与生成视频迁移；闭环实机证据为双臂YAM抽屉三配置各10回合，开放环动作转移仅定性。

[原文入口](https://arxiv.org/abs/2611.05377v1) · [原文 PDF](https://arxiv.org/pdf/2611.05377v1) · [作者项目 / 代码入口](https://cvlab-kaist.github.io/DreamX/) · [作者与团队](../leaderboard/origins/papers/dreamx.md)

版本锁定arXiv v1。96.7%为到达/推闭两个子目标等权平均；各配置10次下推闭28/30。开放环动作转移和生成视频迁移与闭环策略证据分开。

## 先看它做了什么

DreamX用Cosmos-Predict2.5 2B的时空特征直接读出动作latent：每个VAE潜帧分配4个可学习query，最长32个2048维token。编码与解码分别用rank16 LoRA，骨干冻结；解码器从首帧和query重建未来，有机器人标签时另加动作流匹配损失，视频流与动作流不互相注意。预训练混合约2.19k小时人/机器人视频。一个变分瓶颈再把每token压到32维；下游策略由当前画面和文字预测这些code，动作DiT读取latent特征和本体状态，不在控制时生成未来视频。源视频迁移则冻结编码器/解码器，换目标首帧生成视频，或换目标初始状态解码开放环动作。

## 带着什么问题读

**视频重建好为什么未必学会可迁移动作？把动作从视频骨干内部读出，能否把外观留给生成先验，并让控制时少生成一段视频？**

## 为什么值得继续读

问题明确，latent动作接口、生成监督与压缩/策略机制可定位；多数据集probe、1008clip视频迁移、实机子目标与机制消融支持表征贡献。按预印本初读收录，不把Universal题目当跨任务闭环通用能力已证实。

证据入口：Table1公共attentive probe：LARYBench平均归一化动作MSE 0.17对DiLA0.38，分类69.67%对62.25%，32维code后为0.22/67.15；各模型原生时窗与预训练不同。Table2 H&R 21任务×48clip=1008clip，统一19个生成帧：FVD57.44对AdaWorld170.19/VideoWorld2 241.92，LPIPS0.179对0.344/0.299；属于生成视频评估。Table3/5抽屉实机3配置各10次：96.7%是reach/push子目标平均；push80/100/100%对应推闭28/30，Mimic-Video push20/0/0%对应2/30。两方法微调均3万步但预训练不同。Table4同子集RGB-only/RGB+action回归0.24/0.23、分类65.3/64.8。Table7去掉latent条件使CALVIN平均长度2.643降到2.378，但split/回合/seed未列。开放环人到机迁移仅定性；1474对28226ms的测时硬件/采样协议未明，不能拿H200训练卡补作推理硬件。

具身关联：把人类视频的运动信息接到机器人动作表征和策略学习，比较生成像素与生成compact latent的控制接口代价。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[知识星系](../universe/papers/dreamx.md) · [七维评分与雷达](../leaderboard/papers/dreamx/README.md) · [arXiv集锦](../arxiv/README.md#paper-dreamx) · [地图方向](../paper-map/README.md#track-video-action) · [首页](../README.md)

元数据核对：2026-11-05。
