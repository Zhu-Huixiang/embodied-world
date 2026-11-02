# 本篇方法链路 · TouchBridge

TouchBridge让人类手套和Wuji灵巧手共享指尖触觉布局及腕相机视角。Tac-Retarget联合优化两手基座SE(3)与关节，匹配指尖位姿、触觉加权接触中心及活跃taxel支撑，并沿用TopoRetarget的距离加权Laplacian思想建立触觉激活的双手接触图。接触时减弱位姿跟踪，并用响应相关几何位移补偿顺应性。SAM2/ProPainter移除人手、渲染机器人外观，固定场景AprilTag消除头部相机运动后转换动作，用转换后的视觉/状态动作微调GR00T N1.7。触觉只服务离线重定向，不输入运行策略。

TouchBridge让人类手套和Wuji灵巧手共享指尖触觉布局及腕相机视角。Tac-Retarget联合优化两手基座SE(3)与关节，匹配指尖位姿、触觉加权接触中心及活跃taxel支撑，并沿用TopoRetarget的距离加权Laplacian思想建立触觉激活的双手接触图。接触时减弱位姿跟踪，并用响应相关几何位移补偿顺应性。SAM2/ProPainter移除人手、渲染机器人外观，固定场景AprilTag消除头部相机运动后转换动作，用转换后的视觉/状态动作微调GR00T N1.7。触觉只服务离线重定向，不输入运行策略。

[本篇星系](../touchbridge.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/touchbridge.md) · [原文依据](https://arxiv.org/abs/2610.40349v1)
