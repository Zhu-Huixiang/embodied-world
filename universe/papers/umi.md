# UMI 星系

Universal Manipulation Interface: In-The-Wild Robot Teaching Without In-The-Wild Robots

**已精讲** · 操作与动作块

[论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md) · [原文](https://www.roboticsproceedings.org/rss20/p045.html) · [评分卡](../../leaderboard/papers/umi/README.md)

手持夹爪上的相机与位姿追踪记录人类示范，政策学习使用相对末端轨迹而非绑定某机器人底座的绝对坐标。部署时匹配观测与动作延迟，双臂任务再加入夹爪之间的相对位置，以保证示范和执行接口一致。抛掷、杯子摆放、衣物折叠与洗碗实验分别检验这些设计。

## 技术挂点

- [空间表示](../concepts/spatial.md)：保留像素、点、体素或对象相对位置的表示，让预测能接到几何与动作位置。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md#43-pd21相对目标为什么不等于逐步增量)

- [条件生成](../concepts/generation.md)：从一个条件生成多个可能输出，学习图像、视频或动作的分布而非只给一个均值。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md#45-接上diffusion-policy观察怎样变成一段动作)

- [扩散去噪](../concepts/diffusion.md)：训练网络从带噪对象估计噪声或干净目标，生成时从噪声开始迭代恢复样本。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md#45-接上diffusion-policy观察怎样变成一段动作)

- [动作表示](../concepts/action.md)：把位置、姿态、关节或运动轨迹变成模型可预测的对象；表示决定后续解码和控制接口。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md#45-接上diffusion-policy观察怎样变成一段动作)

- [动作块](../concepts/chunk.md)：一次预测多个未来控制时刻的动作，再执行部分并用新观测更新。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md#45-接上diffusion-policy观察怎样变成一段动作)

- [示范模仿](../concepts/imitation.md)：从专家、人类或教师策略的行为学习动作，研究数据、表示和执行误差。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md#45-接上diffusion-policy观察怎样变成一段动作)

- [行为克隆](../concepts/bc.md)：直接监督观测到动作的映射，不必在每次更新中根据奖励搜索。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md#45-接上diffusion-policy观察怎样变成一段动作)

- [机器人数据与评测](../concepts/data.md)：统一观测、动作、任务与评测条件，判断数据多样性如何影响泛化。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md#7-野外泛化把杯子带出训练桌)

- [跨本体数据](../concepts/cross-body.md)：从多个机器人或人类收集经验，通过动作/观测适配接到共享学习系统。 [本篇的具体讲解](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md#61-摆杯视野坐标和跨机械臂)

## 本篇行星与卫星

- [空间表示](umi/spatial.md) · 已讲解
- [条件生成](umi/generation.md) · 已讲解
- [扩散去噪](umi/diffusion.md) · 已讲解
- [动作表示](umi/action.md) · 已讲解
- [动作块](umi/chunk.md) · 已讲解
- [示范模仿](umi/imitation.md) · 已讲解
- [行为克隆](umi/bc.md) · 已讲解
- [机器人数据与评测](umi/data.md) · 已讲解
- [跨本体数据](umi/cross-body.md) · 已讲解
- [本篇方法链路](umi/method-chain.md) · 初读挂点
- [示范数据与可部署数据之间的缺口](umi/method-interface-gap.md) · 已讲解
- [遥操作、被动视频与手持工具](umi/method-three-data-routes.md) · 已讲解
- [让采集与执行看到相近画面](umi/method-wrist-interface.md) · 已讲解
- [155度鱼眼保留上下文](umi/method-fisheye.md) · 已讲解
- [侧镜在单张图内提供隐式立体](umi/method-mirror-stereo.md) · 已讲解
- [翻转镜区并交换左右](umi/method-mirror-swap.md) · 已讲解
- [视觉与惯性共同恢复轨迹](umi/method-visual-inertial.md) · 已讲解
- [共享地图是初始化而非冻结地图](umi/method-map-initialization.md) · 已讲解
- [标记辅助建图不进入示范画面](umi/method-marker-initialization.md) · 已讲解
- [连续夹爪宽度决定松手与接触](umi/method-width.md) · 已讲解
- [软指在末端提供被动顺应](umi/method-compliance.md) · 已讲解
- [采集通用仍需检查目标机器人可达性](umi/method-kinematic-filter.md) · 已讲解
- [按拍摄时刻重新对齐历史](umi/method-observation-time.md) · 已讲解
- [滚动二维码测相机端到端延迟](umi/method-camera-latency.md) · 已讲解
- [本体延迟区分精确时间与近似测法](umi/method-proprio-latency.md) · 已讲解
- [执行延迟从命令与回读对齐估计](umi/method-execution-latency.md) · 已讲解
- [删除已错过执行时刻的动作前缀](umi/method-expired-prefix.md) · 已讲解
- [臂与夹爪提前不同时间发令](umi/method-command-ahead.md) · 已讲解
- [整段未来轨迹共享当前参考帧](umi/method-relative-action.md) · 已讲解
- [本体历史也使用相对位姿](umi/method-relative-history.md) · 已讲解
- [双手需要知道彼此在哪里](umi/method-intergripper.md) · 已讲解
- [用条件去噪学习示范动作序列](umi/method-diffusion-policy.md) · 已讲解
- [视图数量与历史长度分别计数](umi/method-observation-shapes.md) · 已讲解
- [动作horizon与去噪步数不同](umi/method-horizons.md) · 已讲解
- [不同任务采用不同视觉编码器](umi/method-backbones.md) · 已讲解
- [动态任务保原速，准静态任务放慢](umi/method-frequency-speed.md) · 已讲解
- [训练视觉扰动覆盖颜色与小位姿变化](umi/method-augmentation.md) · 已讲解
- [各方法面对人工匹配初态](umi/protocol-initial-states.md) · 已讲解
- [实机评测由人持续监督](umi/protocol-supervision.md) · 已讲解
- [摆杯成功同时约束位置与杯柄方向](umi/experiment-cup.md) · 已讲解
- [同一checkpoint移到另一机械臂](umi/experiment-cross-arm.md) · 已讲解
- [视野消融通过后处理裁切完成](umi/experiment-fisheye.md) · 已讲解
- [绝对动作需要额外全局标定](umi/experiment-action-space.md) · 已讲解
- [同策略时延补偿改变抛掷成功](umi/experiment-tossing.md) · 已讲解
- [扔进桶的计数口径](umi/protocol-toss-success.md) · 已讲解
- [双手相对位姿支持同步抓折](umi/experiment-bimanual.md) · 已讲解
- [折衣采用投影形状判定](umi/protocol-fold-success.md) · 已讲解
- [洗碗恢复动作包含在示范中](umi/experiment-washing.md) · 已讲解
- [视觉比较同时改变预训练与结构](umi/experiment-washing-backbone.md) · 已讲解
- [干净盘子的操作性定义](umi/protocol-cleanliness.md) · 已讲解
- [把杯子示范搬到三十个地点](umi/experiment-wild-data.md) · 已讲解
- [两个未见环境的六十次评估](umi/experiment-wild-eval.md) · 已讲解
- [同骨干仍需要足够丰富的数据](umi/experiment-wild-baseline.md) · 已讲解
- [采集吞吐把重置与故障一起计时](umi/experiment-throughput.md) · 已讲解
- [轨迹均值精度由MoCap对照测量](umi/experiment-tracking.md) · 已讲解
- [低纹理仍会削弱离线动作恢复](umi/limit-texture.md) · 已讲解
- [夹爪重量与自由度限制采集效率](umi/limit-ergonomics.md) · 已讲解
- [接口通用不消除身体约束](umi/limit-interface-generality.md) · 已讲解

## 论文间的联系

- [UMI](umi.md) → [Diffusion Policy](diffusion-policy.md)：UMI所有任务使用Diffusion Policy生成条件动作轨迹，并在附录列出视觉编码器、频率、速度和增强调整。 [原文定位](https://umi-gripper.github.io/umi.pdf)（§III-B p5; App.E pp16–17; bibliography reference[9]）。

- [UMI](umi.md) → [CLIP](clip.md)：UMI的杯子和洗碗策略微调CLIP预训练ViT视觉编码器；抛掷与折衣使用ResNet，不能将全部任务混称CLIP策略。 [原文定位](https://umi-gripper.github.io/umi.pdf)（TableA1 p16; App.E1 p17; RSS §V-D p9 and reference[29] p13）。

[宇宙目录](../README.md) · [论文地图](../../paper-map/README.md) · [具身榜](../../leaderboard/README.md)
