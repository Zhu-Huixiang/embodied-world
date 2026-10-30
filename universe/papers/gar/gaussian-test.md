# 固定观测下的高斯近似 · GAR

给定同一观测，分组拟合教师动作样本并与留出样本比较。

每教师300个context、每个1024样本分512拟合/512留出；平移与旋转各16×3=48维，单独测相对sliced W1，并用高斯重采样给有限样本基线。

[本篇星系](../gar.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/gar.md) · [原文依据](https://arxiv.org/pdf/2610.40271v1)
