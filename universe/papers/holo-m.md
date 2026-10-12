# Holo-M 星系

Humanoid Loco-Manipulation With Discrete VLA Model

**已精讲** · 视觉语言动作模型 VLA

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/holo-m-2609.35709/README.md) · [原文](https://arxiv.org/abs/2609.35709v1) · [评分卡](../../leaderboard/papers/holo-m/README.md)

DCT低频系数与四级残差码固定组长；缺失组监督连接人类/机器人数据，分组恢复接上重叠控制。

## 技术挂点

- [DCT 频率系数](../concepts/dct.md)：把时间序列换到余弦频率基，低频系数描述缓慢变化，高频描述更快变化。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/holo-m-2609.35709/README.md#31-统一动作编码208究竟怎么算出来的)

- [残差向量量化 RVQ](../concepts/rvq.md)：用第一层码近似向量，再用后续码近似剩余误差，最后把各层码相加重建。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/holo-m-2609.35709/README.md#31-统一动作编码208究竟怎么算出来的)

- [动作块](../concepts/chunk.md)：一次预测多个未来控制时刻的动作，再执行部分并用新观测更新。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/holo-m-2609.35709/README.md#31-统一动作编码208究竟怎么算出来的)

- [全身控制与执行](../concepts/wbc.md)：将运动目标、机器人状态和约束转成关节目标或力矩，协调腿、手臂与底盘。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/holo-m-2609.35709/README.md#34-四阶段训练e区让缺标签的数据也能上桌)

- [跨本体数据](../concepts/cross-body.md)：从多个机器人或人类收集经验，通过动作/观测适配接到共享学习系统。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/holo-m-2609.35709/README.md#32-vlm-骨干c区到底往模型里塞了什么)

## 本篇行星与卫星

- [DCT 频率系数](holo-m/dct.md) · 已讲解
- [残差向量量化 RVQ](holo-m/rvq.md) · 已讲解
- [动作块](holo-m/chunk.md) · 已讲解
- [全身控制与执行](holo-m/wbc.md) · 已讲解
- [跨本体数据](holo-m/cross-body.md) · 已讲解
- [本篇方法链路](holo-m/method-chain.md) · 已讲解
- [3.1 统一动作编码：208究竟怎么算出来的？](holo-m/section-3-1.md) · 已讲解
- [3.2 VLM 骨干：C区到底往模型里塞了什么？](holo-m/section-3-2.md) · 已讲解
- [3.3 分组离散扩散：D区从打字改成填空](holo-m/section-3-3.md) · 已讲解
- [3.4 四阶段训练：E区让缺标签的数据也能上桌](holo-m/section-3-4.md) · 已讲解
- [4.1 先把评测的单位讲清楚](holo-m/section-4-1.md) · 已讲解
- [4.2 Generalist：总分涨了，这格怎么掉了？](holo-m/section-4-2.md) · 已讲解
- [4.3 Specialist：专门练之后，移动抓取怎样？](holo-m/section-4-3.md) · 已讲解
- [4.4 数据消融：A区那批人的手，帮了多少忙？](holo-m/section-4-4.md) · 已讲解
- [4.5 实机部署：F区，时钟开始较真了](holo-m/section-4-5.md) · 已讲解

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
