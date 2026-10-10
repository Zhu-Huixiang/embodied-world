# Flow Straight and Fast: Learning to Generate and Transfer Data with Rectified Flow

出处：ICLR 2023。研究范围：生成/表征基础，动作/视频流模型的直线路径与少步生成。

[原文入口](https://iclr.cc/virtual/2023/poster/11266) · [原文 PDF](https://openreview.net/pdf?id=gWxpdtQpiYV) · [作者项目 / 代码入口](https://github.com/gnobitab/RectifiedFlow)

ICLR 2023 正式论文；与 Flow Matching 的目标和 reflow 操作分别说明。

阅读问题：**训练速度场和把轨迹拉直有什么区别，为什么直一点就能少算几步？**

收录理由：线性插值回归及 reflow 把数值求解误差与路径弯曲联系起来，有助于理解具身连续动作生成中的少步速度取舍。

证据入口：线性路径、传输性质与反复拉直的机制可单独解释，官方代码公开；适合比较连续动作生成里少步求解的理论和代价。

具身关联：线性插值回归及 reflow 把数值求解误差与路径弯曲联系起来，有助于理解具身连续动作生成中的少步速度取舍。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/rectified-flow/README.md)

机制简析：从两个分布采样端点，用连接端点的线性插值训练速度场，让网络按当前位置估计路径速度。再用已有流生成配对数据重新训练，逐步减少轨迹弯曲，使粗时间步的数值积分更准确。原文给出传输代价性质，并在图像生成和域迁移中比较一步与多步效果。
<!-- discovery:end -->
