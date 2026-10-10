# Elucidating the Design Space of Diffusion-Based Generative Models

**解读导读** · NeurIPS 2022 · [Diffusion / Transformer 基础](../paper-map/README.md#track-diffusion-transformer)

研究范围：生成/表征基础，动作/视频扩散的噪声参数化与推理成本诊断。

[原文入口](https://proceedings.neurips.cc/paper_files/paper/2022/hash/a98846e9d9cc01cfb87eb694d946ce6b-Abstract-Conference.html) · [原文 PDF](https://proceedings.neurips.cc/paper_files/paper/2022/file/a98846e9d9cc01cfb87eb694d946ce6b-Paper-Conference.pdf) · [作者项目 / 代码入口](https://github.com/NVlabs/edm) · [作者与团队](../leaderboard/origins/papers/edm.md)

NeurIPS 2022；原文研究图像生成，具身用途定位为采样与训练设计基础。

## 先看它做了什么

把扩散过程的噪声参数化、采样求解器和网络预处理分别定义，减少不同实现之间的隐性差异。网络输入、输出和训练损失按噪声尺度预调节，推理使用更合适的时间离散与高阶求解。原文同时重用旧模型更换采样器、重训网络，比较质量与网络调用次数。

## 带着什么问题读

**同样是扩散，噪声尺度、网络预处理和数值求解器各改变了哪一层？**

## 为什么值得继续读

将常被混用的采样、噪声日程与网络预处理拆开，能帮助分析动作生成速度及视频模型的稳定性，公开实现可逐项测试。

证据入口：模块化贡献配有重用旧网络和重新训练的对照，速度质量证据扎实，官方实现让设计取舍可操作。

具身关联：将常被混用的采样、噪声日程与网络预处理拆开，能帮助分析动作生成速度及视频模型的稳定性，公开实现可逐项测试。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[七维评分与雷达](../leaderboard/papers/edm/README.md) · [NeurIPS集锦](../venues/NeurIPS/README.md) · [地图方向](../paper-map/README.md#track-diffusion-transformer) · [首页](../README.md)

元数据核对：2026-10-10。
