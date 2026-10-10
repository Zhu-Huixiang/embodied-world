# Emerging Properties in Self-Supervised Vision Transformers

出处：ICCV 2021。研究范围：生成/表征基础，DINOv2 与具身模型冻结视觉特征的自蒸馏起点。

[原文入口](https://openaccess.thecvf.com/content/ICCV2021/html/Caron_Emerging_Properties_in_Self-Supervised_Vision_Transformers_ICCV_2021_paper.html) · [原文 PDF](https://openaccess.thecvf.com/content/ICCV2021/papers/Caron_Emerging_Properties_in_Self-Supervised_Vision_Transformers_ICCV_2021_paper.pdf) · [作者项目 / 代码入口](https://github.com/facebookresearch/dino)

ICCV 2021，会议为 2021-10-10 至 2021-10-17，正式会议日期位于五年窗口边界；首次预印本早于会议。

阅读问题：**没有人工标签，教师与学生互相对齐怎么还能长出物体边界？**

收录理由：无标签自蒸馏及其空间特征是 DINOv2 的直接前身，DINOv2 再进入 OpenVLA；按正式会议时间收录并保留首次公开日期区别。

证据入口：动量教师、裁剪与防坍塌措施能逐项分析，视觉迁移和空间结构有原始实验支撑，官方实现可复用。

具身关联：无标签自蒸馏及其空间特征是 DINOv2 的直接前身，DINOv2 再进入 OpenVLA；按正式会议时间收录并保留首次公开日期区别。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/dino/README.md)

机制简析：同一图像的不同裁剪分别进入学生和教师，学生用交叉熵拟合教师输出的概率分布。教师参数由学生参数的指数滑动平均更新，中心化与温度锐化防止两者退化成常量。原文比较 ViT 与卷积网络，检查 k-NN、线性分类和注意力中出现的物体区域结构。
<!-- discovery:end -->
