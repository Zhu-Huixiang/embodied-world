# VC-1 星系

Where are we in the search for an Artificial Visual Cortex for Embodied Intelligence?

**导读** · 具身感知与场景表示

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/vc1.md) · [原文](https://proceedings.neurips.cc/paper_files/paper/2023/hash/022ca1bed6b574b962c48a2856eb207b-Abstract-Conference.html) · [评分卡](../../leaderboard/papers/vc1/README.md)

先把导航、移动操作、灵巧操作和运动控制纳入 CortexBench，统一比较不同预训练视觉模型。固定 MAE 目标后变化视频来源、数据规模和 ViT 容量，再检验同一编码器能否处处占优。VC-1 的平均提升和任务适配提升分别报告，暴露视觉预训练的任务差异。

## 技术挂点

- [遮蔽预测](../concepts/masking.md)：隐藏部分输入，训练模型恢复像素、token 或表征。恢复什么决定监督重点。

- [视觉 patch token](../concepts/patches.md)：把图像切成块，展平并投影成向量，再加入位置信息。

- [泛化评测与遗忘](../concepts/benchmark.md)：拆开任务、物体、场景或学习顺序，检查迁移能力和旧技能保留。

## 本篇行星与卫星

- [遮蔽预测](vc1/masking.md) · 初读挂点
- [视觉 patch token](vc1/patches.md) · 初读挂点
- [泛化评测与遗忘](vc1/benchmark.md) · 初读挂点
- [本篇方法链路](vc1/method-chain.md) · 初读挂点

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
