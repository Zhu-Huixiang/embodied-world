# 视觉与惯性共同恢复轨迹 · UMI

GoPro的RGB和内置加速度计、陀螺仪进入visual-inertial SLAM，恢复有公制尺度的相机运动。

IMU能短时支撑视觉模糊或纹理不足时的追踪，不能据此宣称任意长时失明也可靠。SLAM用于离线数据处理。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md#33-hd4视频怎样长出以米为单位的轨迹)

继续拆：[共享地图是初始化而非冻结地图](method-map-initialization.md)。

[本篇星系](../umi.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md) · [原文依据](https://www.roboticsproceedings.org/rss20/p045.pdf)
