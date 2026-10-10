# Ctrl-World: A Controllable Generative World Model for Robot Manipulation

**解读导读** · ICLR 2026 · [世界模型与模型强化学习](../paper-map/README.md#track-world-model)

研究范围：操作世界模型；VLA评估与合成回训。

[原文入口](https://proceedings.iclr.cc/paper_files/paper/2026/hash/0ae94013da7cd459402fd77874e09ee3-Abstract-Conference.html) · [原文 PDF](https://arxiv.org/pdf/2510.10125v1) · [作者项目 / 代码入口](https://ctrl-world.github.io/)

ICLR2026正式论文；作者预印本v1首次公开2025-10-11。合成数据改进的38.7%→83.4%为44.7个百分点。

## 先看它做了什么

1.5B SVD初始化，多相机token联合生成；稀疏历史图像带机器人姿态通过逐帧cross-attention检索；未来动作转换笛卡尔姿态后逐帧条件化。策略在模型里闭环rollout，人工筛成功轨迹再微调VLA。

## 带着什么问题读

**怎样让视频生成器按真实动作走，并使想象中的策略排名接近实机？**

## 为什么值得继续读

可核正式主会、模块消融、实机对照和开源模型评价闭环齐备。

证据入口：95,599条DROID轨迹/564场景训练；留出2%轨迹，256片段十秒自回归生成；完整模型third-view FVD97.4，去memory105.5，去逐帧条件122.7。（Table 1-2 / §5.1-5.2）；三公开策略π0、π0-FAST、π0.5，7类任务，同起始图像对比模型/实机；指令遵循回归y=0.87x-0.04，任务成功y=0.81x-0.11；模型倾向低估低层成功。（§5.3 / Fig.7）；每任务合成400轨迹，人工保留25–50条成功样本，微调2000steps；陌生物体/指令的实机成功38.7%→83.4%。（§5.4 / Fig.9）

具身关联：操作世界模型；VLA评估与合成回训；怎样让视频生成器按真实动作走，并使想象中的策略排名接近实机？

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/ctrl-world/README.md) · [ICLR集锦](../venues/ICLR/README.md) · [地图方向](../paper-map/README.md#track-world-model) · [首页](../README.md)

元数据核对：2026-10-10。
