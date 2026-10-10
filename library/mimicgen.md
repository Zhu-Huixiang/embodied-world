# MimicGen: A Data Generation System for Scalable Robot Learning using Human Demonstrations

出处：CoRL 2023。研究范围：对象中心轨迹变换与自动机器人示范生成。

[原文入口](https://proceedings.mlr.press/v229/mandlekar23a.html) · [原文 PDF](https://proceedings.mlr.press/v229/mandlekar23a/mandlekar23a.pdf) · [作者项目 / 代码入口](https://mimicgen.github.io/)

CoRL 2023 正式版；生成需对象位姿及子任务结构假设，不能写成对任意人类视频自由扩增。

阅读问题：**把十条示范扩成上千条，什么时候是有用的新数据，什么时候只是机械复制？**

收录理由：机器人合成示范数据的代表技术，长任务、精密操作、多对象与跨机器人实验扎实，公开系统被后续模拟数据工作使用。

证据入口：CoRL PDF 明确动作和对象假设，提供跨任务/模拟器/硬件生成、初始分布和示范质量研究；项目公开生成代码、数据和环境，复用价值很高。

具身关联：机器人合成示范数据的代表技术，长任务、精密操作、多对象与跨机器人实验扎实，公开系统被后续模拟数据工作使用。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/mimicgen/README.md)

机制简析：源示范按对象中心子任务切段；新场景中选择源段，按对象的新位姿变换末端轨迹，再拼接并实际执行。执行成功才把状态和动作加入生成数据，而不是只复制一组数学坐标。原文逐步扩大初始状态分布、替换物体与机械臂，并比较生成示范和追加同量人类示范的策略表现。
<!-- discovery:end -->
