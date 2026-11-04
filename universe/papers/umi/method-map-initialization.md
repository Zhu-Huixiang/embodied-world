# 共享地图是初始化而非冻结地图 · UMI

每场景先建图，后续示范重定位到已有地图后继续正常SLAM建图和优化。

只锁定地图的localization模式难以应付操作改变物体位置；作者修改的是重定位后的系统行为。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md#33-hd4视频怎样长出以米为单位的轨迹)

继续拆：[标记辅助建图不进入示范画面](method-marker-initialization.md)。

[本篇星系](../umi.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md) · [原文依据](https://umi-gripper.github.io/umi.pdf)
