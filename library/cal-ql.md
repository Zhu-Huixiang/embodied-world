# Cal-QL: Calibrated Offline RL Pre-Training for Efficient Online Fine-Tuning

**解读导读** · NeurIPS 2023 · [强化学习与离线决策](../paper-map/README.md#track-reinforcement-learning)

研究范围：离线到在线 RL；视觉操作和导航。

[原文入口](https://proceedings.neurips.cc/paper_files/paper/2023/hash/c44a04289beaf0a7d968a94066a1d696-Abstract-Conference.html) · [原文 PDF](https://proceedings.neurips.cc/paper_files/paper/2023/file/c44a04289beaf0a7d968a94066a1d696-Paper-Conference.pdf) · [作者项目 / 代码入口](https://nakamotoo.github.io/Cal-QL)

## 先看它做了什么

Cal-QL 保留 CQL 的保守价值学习，同时把学习策略的价值锚定在一个可估计参考策略的价值之上。这样在线新数据进入时，低估的旧 Q 不至于诱导策略先丢掉离线技能。原文分别分析初期遗忘、价值尺度变化，并在导航、操作和图像输入微调任务上比较。

## 带着什么问题读

**离线训练把 Q 压得太低，为什么一上真环境反而会先忘掉已有技能？**

## 为什么值得继续读

把离线预训练与在线微调的失效现象具体化，连接真实机器人有限交互问题，且有 CQL/IQL/TD3+BC 对照。

证据入口：先诊断再设计算法，含多个离线到在线域、理论条件、基线和校准消融，适合作为机器人预训练后的 RL 入门。

具身关联：把离线预训练与在线微调的失效现象具体化，连接真实机器人有限交互问题，且有 CQL/IQL/TD3+BC 对照。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/cal-ql/README.md) · [NeurIPS集锦](../venues/NeurIPS/README.md) · [地图方向](../paper-map/README.md#track-reinforcement-learning) · [首页](../README.md)

元数据核对：2026-10-10。
