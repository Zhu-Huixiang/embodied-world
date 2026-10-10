# Learning Universal Policies via Text-Guided Video Generation

**解读导读** · NeurIPS 2023 · [视频动作模型与视觉推理](../paper-map/README.md#track-video-action)

研究范围：UniPi、视频扩散规划与逆动力学控制。

[原文入口](https://proceedings.neurips.cc/paper_files/paper/2023/hash/1d5b9233ad716a43be5c0d3023cb82d0-Abstract-Conference.html) · [原文 PDF](https://proceedings.neurips.cc/paper_files/paper/2023/file/1d5b9233ad716a43be5c0d3023cb82d0-Paper-Conference.pdf) · [作者项目 / 代码入口](https://universal-policy.github.io/)

NeurIPS 2023。互联网视频迁移段包含视觉计划生成，不能一概写成真实机器人闭环执行证明。项目页此次 Exa fetch 失败，方法与实验使用正式 PDF。

## 先看它做了什么

当前图像和文字任务条件送入视频扩散模型，生成未来画面序列作为计划；逆动力学模型再从相邻或计划帧回归环境专用动作。计划能先生成稀疏关键帧再细化，也可在采样时施加额外约束。原文在组合泛化、多任务与层级规划上评估，并探索互联网视频知识迁移。

## 带着什么问题读

**先生成机器人会怎么做的视频，再倒推出动作，这条路线解决了什么又把难题搬到了哪里？**

## 为什么值得继续读

视频生成作为统一规划空间的早期代表工作，直接连接世界模型、视频动作模型与机器人控制。

证据入口：NeurIPS PDF 定义统一预测决策过程、视频到动作接口和分层采样，并分别评估组合与跨任务能力；控制与可见视频计划要分层看，实机证据评分较谨慎。

具身关联：视频生成作为统一规划空间的早期代表工作，直接连接世界模型、视频动作模型与机器人控制。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/unipi/README.md) · [NeurIPS集锦](../venues/NeurIPS/README.md) · [地图方向](../paper-map/README.md#track-video-action) · [首页](../README.md)

元数据核对：2026-10-10。
