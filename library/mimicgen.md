# MimicGen: A Data Generation System for Scalable Robot Learning using Human Demonstrations

**解读导读** · CoRL 2023 · [操作与动作块](../paper-map/README.md#track-manipulation)

研究范围：对象中心轨迹变换与自动机器人示范生成。

[原文入口](https://proceedings.mlr.press/v229/mandlekar23a.html) · [原文 PDF](https://proceedings.mlr.press/v229/mandlekar23a/mandlekar23a.pdf) · [作者项目 / 代码入口](https://mimicgen.github.io/) · [作者与团队](../leaderboard/origins/papers/mimicgen.md)

CoRL 2023 正式版；生成需对象位姿及子任务结构假设，不能写成对任意人类视频自由扩增。

## 先看它做了什么

源示范按对象中心子任务切段；新场景中选择源段，按对象的新位姿变换末端轨迹，再拼接并实际执行。执行成功才把状态和动作加入生成数据，而不是只复制一组数学坐标。原文逐步扩大初始状态分布、替换物体与机械臂，并比较生成示范和追加同量人类示范的策略表现。

## 带着什么问题读

**把十条示范扩成上千条，什么时候是有用的新数据，什么时候只是机械复制？**

## 为什么值得继续读

机器人合成示范数据的代表技术，长任务、精密操作、多对象与跨机器人实验扎实，公开系统被后续模拟数据工作使用。

证据入口：CoRL PDF 明确动作和对象假设，提供跨任务/模拟器/硬件生成、初始分布和示范质量研究；项目公开生成代码、数据和环境，复用价值很高。

具身关联：机器人合成示范数据的代表技术，长任务、精密操作、多对象与跨机器人实验扎实，公开系统被后续模拟数据工作使用。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/mimicgen/README.md) · [CoRL集锦](../venues/CoRL/README.md) · [地图方向](../paper-map/README.md#track-manipulation) · [首页](../README.md)

元数据核对：2026-10-10。
