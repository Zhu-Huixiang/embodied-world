# 包围盒剪枝与半段距离复用 · cuRoboV2-Fast

先用廉价边界剔除不相交连杆或远处障碍。

自碰撞按连杆AABB剪枝，世界碰撞共用相邻half-sweep端点距离并合并梯度；仍受选定采样分辨率约束。

[本篇星系](../curobov2-fast.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/curobov2-fast.md) · [原文依据](https://arxiv.org/pdf/2611.06913v1)
