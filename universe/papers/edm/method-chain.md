# 本篇方法链路 · EDM

把扩散过程的噪声参数化、采样求解器和网络预处理分别定义，减少不同实现之间的隐性差异。网络输入、输出和训练损失按噪声尺度预调节，推理使用更合适的时间离散与高阶求解。原文同时重用旧模型更换采样器、重训网络，比较质量与网络调用次数。

把扩散过程的噪声参数化、采样求解器和网络预处理分别定义，减少不同实现之间的隐性差异。网络输入、输出和训练损失按噪声尺度预调节，推理使用更合适的时间离散与高阶求解。原文同时重用旧模型更换采样器、重训网络，比较质量与网络调用次数。

[本篇星系](../edm.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/edm.md) · [原文依据](https://proceedings.neurips.cc/paper_files/paper/2022/hash/a98846e9d9cc01cfb87eb694d946ce6b-Abstract-Conference.html)
