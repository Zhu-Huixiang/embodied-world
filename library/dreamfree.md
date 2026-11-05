# Future Representation Distillation for Imagination-Free World Action Models

**解读导读** · arXiv 2026 · [世界动作模型](../paper-map/README.md#track-world-action-model)

研究范围：LIBERO、RoboCasa和RoboTwin仿真；DROID10任务×5次/方法实机，YAM双臂另训后仅定性。任务内新物体/布置不混作未见任务泛化。

[原文入口](https://arxiv.org/abs/2611.04527v1) · [原文 PDF](https://arxiv.org/pdf/2611.04527v1) · [作者项目 / 代码入口](https://harryjo97.github.io/dreamfree/) · [作者与团队](../leaderboard/origins/papers/dreamfree.md)

## 先看它做了什么

先对机器人视频适配Wan，再冻结教师；学生用注意力mask让当前token只读当前观测和指令，投影成未来布局，与看过带噪真实未来的教师token做余弦蒸馏，同时保留视频流匹配正则。第二阶段冻结视觉编码器，用64个query读出预测特征，约1B动作DiT条件于指令、本体和DROID动作历史学流匹配。运行只单次视觉编码，动作仍去噪10或16步，输出32动作并执行指定前缀。

## 带着什么问题读

**视频模型知道一些将来会发生什么，控制器是否必须先把未来逐帧画出来，还是能把预测知识压进当前帧表征？**

## 为什么值得继续读

目标不是泛泛加一个世界模型，而是解决视频去噪开销与动作所需预测信息不匹配；显式蒸馏的消融、特征探针、规模/视频数据与实机证据共同支持有实质贡献的初读收录。

证据入口：RoboCasa24任务各50评测试次：14B71.7%，自训Fast-WAM14B44.7%；去蒸馏47.2、去生成55.6。其他基线如CosmosPolicy67.1为引用结果。DROID10×5实机：64%对DreamZero56%与pi0.5 16%，按各公开checkpoint设置；YAM只定性。单H200暖机后91ms/chunk对1632ms，排除通信/执行，不把倒数11Hz当24动作执行后的完整闭环频率。RoboTwin跨本体视频迁移三任务各20次平均6.7→30%，仍需原子任务动作标签。

具身关联：直接连接预训练视频模型与视觉闭环操作；区分视频生成、预测表示、动作去噪与执行窗口。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[知识星系](../universe/papers/dreamfree.md) · [七维评分与雷达](../leaderboard/papers/dreamfree/README.md) · [arXiv集锦](../arxiv/README.md#paper-dreamfree) · [地图方向](../paper-map/README.md#track-world-action-model) · [首页](../README.md)

元数据核对：2026-11-05。
