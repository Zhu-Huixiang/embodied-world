# 动作表示

把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。

动作单位、参考系与时间频率比“统一 token”四个字更具体。

继续拆：[动作块](chunk.md) · [离散编码与量化](quantization.md) · [DCT 频率系数](dct.md) · [运动重定向](retarget.md) · [全身控制与执行](wbc.md)。

## 哪些论文用到或讨论它

- [CoT-VLA](../papers/cot-vla.md) · 机制导读 · [原文](https://openaccess.thecvf.com/content/CVPR2025/html/Zhao_CoT-VLA_Visual_Chain-of-Thought_Reasoning_for_Vision-Language-Action_Models_CVPR_2025_paper.html)
- [DreamZero](../papers/dreamzero.md) · 机制导读 · [原文](https://arxiv.org/abs/2602.15922)
- [VideoVLA](../papers/videovla.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2025/hash/89a3b655a8b68ae1c76b768152c9c19d-Abstract-Conference.html)
- [Open X-Embodiment](../papers/rtx.md) · 机制导读 · [原文](https://ieeexplore.ieee.org/document/10611477)
- [UMI](../papers/umi.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss20/p045.html)
- [Transporter](../papers/transporter.md) · 机制导读 · [原文](https://proceedings.mlr.press/v155/zeng21a.html)
- [Decision Transformer](../papers/decision-transformer.md) · 机制导读 · [原文](https://proceedings.neurips.cc/paper_files/paper/2021/hash/7f489f642a0ddb10272b5c31057f0663-Abstract.html)
- [Diffuser](../papers/diffuser.md) · 机制导读 · [原文](https://proceedings.mlr.press/v162/janner22a.html)
- [Walk These Ways](../papers/walk-these-ways.md) · 机制导读 · [原文](https://proceedings.mlr.press/v205/margolis23a.html)
- [Walk in the Park](../papers/walk-in-the-park.md) · 机制导读 · [原文](https://www.roboticsproceedings.org/rss19/p056.html)
- [FLoRe](../papers/flore.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.35862v1)
- [JAM](../papers/jam.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.37219v1)
- [TOPS](../papers/tops.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.36694v1)
- [ARC](../papers/arc.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.12386v1)
- [PLaW-VLA](../papers/plaw-vla.md) · 机制导读 · [原文](https://arxiv.org/abs/2610.12285v1)

每篇的用法需要放回它自己的输入、损失与任务条件理解。这里按已有机制台账建立技术导航，完整讲解以亮起的章节为入口。

[宇宙目录](../README.md) · [知识图谱](https://zhu-huixiang.github.io/embodied-world/universe/)
