# LeWorldModel: Stable End-to-End Joint-Embedding Predictive Architecture from Pixels

出处：arXiv 2026。研究范围：潜世界模型；无奖励离线视觉规划。

[原文入口](https://arxiv.org/abs/2603.19312v1) · [原文 PDF](https://arxiv.org/pdf/2603.19312v1) · [作者项目 / 代码入口](https://le-wm.github.io/)

官方arXiv Submission history核实v1首投2026-03-13 19:48:14 UTC（上海2026-03-14 03:48:14）；最新已发现v3，当前科学摘录仍读v1。LeWAM是另篇联合世界动作模型，不能按名称合并。

阅读问题：**两项损失怎样让像素JEPA不坍缩，又把每帧压成一个可规划的token？**

收录理由：防坍缩目标、同FLOPs规划与公开可复用实现都有明确证据。

证据入口：50 runs平均完整规划时间LeWM 0.98s vs DINO-WM 47s；固定FLOPs PushT成功率90% vs 13%，OGB-Cube74% vs48%。（Fig.3）；Push-T LeWM96%、PLDM78%、DINO-WM74%；Two-Room LeWM87%而多baseline100%；OGBench-Cube LeWM74%低于DINO-WM86%。（Fig.6）；嵌入维度/随机投影数/积分节点消融；lambda∈[0.01,0.2] PushT成功率保持80%以上，而lambda0.5下降。（Fig.15-16; Appendix G）

具身关联：潜世界模型；无奖励离线视觉规划；两项损失怎样让像素JEPA不坍缩，又把每帧压成一个可规划的token？

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/lewm/README.md)

机制简析：ViT将每帧变成192维CLS表征；动作AdaLN条件的Transformer预测下个latent。MSE预测+SIGReg随机投影高斯正则共同训练，无EMA/stop-gradient/重建。部署用latent目标距离和CEM选动作，再MPC重规划。
<!-- discovery:end -->
