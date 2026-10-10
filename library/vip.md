# VIP: Towards Universal Visual Reward and Representation via Value-Implicit Pre-Training

出处：ICLR 2023。研究范围：人类视频、隐式价值预训练与视觉奖励。

[原文入口](https://openreview.net/forum?id=YJ7o2wetJ2) · [原文 PDF](https://openreview.net/pdf?id=YJ7o2wetJ2) · [作者项目 / 代码入口](https://sites.google.com/view/vip-rl)

ICLR 2023 主会见官方 poster 页；OpenReview 当前反爬返回校验页，方法初读使用作者项目与 arXiv。VZIKjcWQxk 是 NeurIPS 2022 workshop 重复入口，不能当 ICLR 录用证据。

阅读问题：**两张图在 latent 空间的距离，为什么可以变成机器人离目标还有多远的奖励？**

收录理由：视觉表征兼作奖励的代表方法，有从离线目标价值学习推导到无动作人类视频预训练的明确理论与实机落点。

证据入口：ICLR 官方页面确认主会，原项目与作者稿提供推导、平滑奖励、控制方法和真实任务对照；代码及 TorchRL 接入给出复用路径。

具身关联：视觉表征兼作奖励的代表方法，有从离线目标价值学习推导到无动作人类视频预训练的明确理论与实机落点。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/vip/README.md)

机制简析：把无动作视频看成目标条件价值学习，再从离线 RL 的对偶目标导出仅需要画面序列的预训练损失。价值隐式地由当前图像与目标图像的嵌入距离表达，因而距离变化能提供稠密视觉奖励。原文检验轨迹优化、在线 RL 与少量真实轨迹的离线 RL，强调表征和奖励同时影响控制。
<!-- discovery:end -->
