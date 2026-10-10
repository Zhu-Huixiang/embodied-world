# RVT-2: Learning Precise Manipulation from Few Demonstrations

出处：RSS 2024。研究范围：粗到细多视图操作、精密插入与系统效率。

[原文入口](https://www.roboticsproceedings.org/rss20/p055.html) · [原文 PDF](https://www.roboticsproceedings.org/rss20/p055.pdf) · [作者项目 / 代码入口](https://robotic-view-transformer-2.github.io/)

RSS 2024；项目标题 Few Examples 与正式论文 Few Demonstrations 同一工作。不同训练设置的 RLBench 数字应逐表引用。

阅读问题：**粗视图定位之后再放大，怎样改善毫米级插入，而不是只让网络更快？**

收录理由：高效 3D 多任务策略由粗操作走向精密插入的代表工作，提供清楚的架构与系统级改进。

证据入口：RSS PDF 提供粗到细结构、位置条件旋转和系统优化消融，以及十示范量级的实机精密任务；属于高质量迭代而非全新范式，因此创新分适度。

具身关联：高效 3D 多任务策略由粗操作走向精密插入的代表工作，提供清楚的架构与系统级改进。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/rvt2/README.md)

机制简析：第一阶段在全场景虚拟视图中估计目标，第二阶段放大局部区域后预测更精确的位置；旋转预测改用目标位置附近特征，避免同场景多个物体方向冲突。凸上采样、较少视图和高效点云渲染控制计算成本。原文分别做这些部件的消融，并用插头和不同孔径 peg 的实机任务检验精度。
<!-- discovery:end -->
