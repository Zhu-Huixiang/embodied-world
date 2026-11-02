# JEDI: Joint-Embedding Demonstration Compression for In-Context Imitation Learning

**解读导读** · arXiv 2026 · [视觉语言动作模型 VLA](../paper-map/README.md#track-vla)

研究范围：以查询未来预测训练示范压缩器的上下文模仿学习；自定义LIBERO/RLBench未见任务拆分及单平台真实双臂实验。

[原文入口](https://arxiv.org/abs/2610.40356v1) · [原文 PDF](https://arxiv.org/pdf/2610.40356v1) · [作者与团队](../leaderboard/origins/papers/jedi.md)

## 先看它做了什么

每段示范由4层Perceiver独立压成8个slot并缓存；π0的flow-matching动作专家读取查询观测与这些slot。辅助预测器在冻结V-JEPA2.1空间预测查询回合下一关键帧，对当前观测支路stop-gradient，使预测损失真正训练示范压缩器。错误任务和同任务不同过程的反事实margin约束保留目标/顺序。用示范间交叉预测误差和查询初图相似性选取一致示范，支持阶段性commitment；人类视频扩展经同平台真实posttraining，用手/物体关键点补充对应，不是任意人类视频免训练通用控制。

## 带着什么问题读

**把一段演示压成几个token，怎么保证保留下来的正好是当前机器人要用的信息？让压缩结果预测当前回合的下一关键帧，能否同时保住目标和执行次序？**

## 为什么值得继续读

压缩目标从只拟合动作变为保留查询未来所需的信息，任务/过程反事实与匹配label控制直接检验示范内容是否被使用；有matched objective、多seed仿真、成本与匹配实机控制，足以有边界收录。

证据入口：Table3同backbone/data/schedule的N8成功率action-only64.2%→JEDI80.2%，CFR34.1→74.9，order match52.2→84.1；label contrast73.5 order match仍低于84.1，支持未来预测的作用。标准实验实际每seed每LIBERO suite随机6任务训练/4任务heldout，共3seed、每任务100rollouts；非标准LIBERO榜。Table9放开观测梯度N8得83.9高于默认80.2，stop-gradient为隔离压缩接口，不能说性能最优。Table2 mixed55→62是共享终点成功率，不是order-match。Table5实机人类N8为21/25、8/10、10/15，N1比较混入上下文数量变化；Table14匹配8条人类示范的40次控制，JEDI各子组15/20、8/10、5/10，对action-only11/20、5/10、2/10。需10任务各8条机器人与8条人类示范的3k步posttraining；测试10新任务仅上下文适应。Table12单A100缓存后N16 13Hz、75ms prefill、11GB；50示范bank还需15s缓存后构建或28s含图像编码。

具身关联：连接VLA动作生成、JEPA预测表示、上下文模仿和人类示范，用机器人闭环任务检验压缩是否保留可执行信息。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[知识星系](../universe/papers/jedi.md) · [七维评分与雷达](../leaderboard/papers/jedi/README.md) · [arXiv集锦](../arxiv/README.md#paper-jedi) · [地图方向](../paper-map/README.md#track-vla) · [首页](../README.md)

元数据核对：2026-11-02。
