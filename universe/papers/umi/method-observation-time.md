# 按拍摄时刻重新对齐历史 · UMI

视觉流通常最迟到达，机器人端按图像真实拍摄时间插值机械臂和夹爪本体观测。

这会让各流描述同一过去时刻；它没有降低相机实际传输时间。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md#41-pd11把各路观测拨到同一个时刻)

继续拆：[滚动二维码测相机端到端延迟](method-camera-latency.md) · [本体延迟区分精确时间与近似测法](method-proprio-latency.md) · [执行延迟从命令与回读对齐估计](method-execution-latency.md)。

[本篇星系](../umi.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/umi-2402.10329/README.md) · [原文依据](https://www.roboticsproceedings.org/rss20/p045.pdf)
