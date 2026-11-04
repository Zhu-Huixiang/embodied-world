# 滚动二维码测相机端到端延迟 · UMI

接收时间减二维码显示时间，再减显示刷新延迟，得到相机链路延迟。

二维码编码的是全局时间；若不扣除显示器延迟，会把屏幕刷新也算进相机传输。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md#42-pd12动作算出来还得来得及执行)

[本篇星系](../umi.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md) · [原文依据](https://umi-gripper.github.io/umi.pdf)
