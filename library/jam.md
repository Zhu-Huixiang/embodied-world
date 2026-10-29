# Vision-Language-Action or World-Action? Just Action Models

**解读导读** · arXiv 2026 · [视觉语言动作模型 VLA](../paper-map/README.md#track-vla)

研究范围：训练期未来表征监督与动作策略；LIBERO、LIBEROPlus及RoboTwin仿真。

[原文入口](https://arxiv.org/abs/2610.37219v1) · [原文 PDF](https://arxiv.org/pdf/2610.37219v1) · [作者项目 / 代码入口](https://y0uroy.github.io/JAM/) · [作者与团队](../leaderboard/origins/papers/jam.md)

## 先看它做了什么

JAM把骨干初始化、未来监督和部署模块拆开：当前图像/语言经骨干提供视觉token，动作专家结合状态生成动作块。训练时，记录的未来只送入冻结anchor得到目标；一个额外prediction head从当前特征预测这些目标，以逐token/时间偏移的余弦距离加动作flow-matching损失训练，目标停止梯度。部署删除anchor和prediction head，动作路径不读未来，也不生成未来图像。固定未来目标可提前缓存；Wan配置以VAE直接编码目标最好，Ovis配置则用Yak特征，不能把结论简化成越大的未来模型越好。

## 带着什么问题读

**VLA和WAM到底差在预训练起点，还是怎样利用未来？把未来监督留下、把视觉生成删掉，控制还会好吗？**

## 为什么值得继续读

把生成式骨干与视觉语言骨干放进同一动作学习框架，做目标设计、跨骨干、扰动、成本与训练种子检查，能追问未来监督究竟在帮哪一步。

证据入口：Table 1：Wan的LIBERO/LIBEROPlus由FastWAM的97.00/55.31变为JAM的98.15/64.54；Ovis由ImageWAM的92.90/65.27变为96.75/79.95。LIBERO为40任务各50次；LIBEROPlus是共享的1506任务固定子集各一次。Table 9：缓存后Wan在线训练FLOPs由15.52降至4.19 TFLOPs/sample/update，约73%，不含一次目标提取；所profile算子GPU时间0.789→0.258秒。Table 20任务bootstrap与Table 21三训练run补不确定度。全部控制实验为仿真。

具身关联：直接检查机器人动作策略怎样利用视觉预训练和未来监督，为VLA/WAM的训练设计提供可拆分的比较。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[知识星系](../universe/papers/jam.md) · [七维评分与雷达](../leaderboard/papers/jam/README.md) · [arXiv集锦](../arxiv/README.md#paper-jam) · [地图方向](../paper-map/README.md#track-vla) · [首页](../README.md)

元数据核对：2026-10-29。
