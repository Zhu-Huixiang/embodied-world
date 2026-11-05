# 编码用文字，重建用latent · DreamX

编码器保留视频骨干的文字交叉注意力，解码器以动作latent替代文字条件。

Q=E(q;V,l)把视频和指令变成latent；解码器从V0与Q重建未来，使额外条件倾向保留解释运动的信息。

继续拆：[同一latent换一个起始画面](dx-video-transfer.md)。

[本篇星系](../dreamx.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/dreamx.md) · [原文依据](https://arxiv.org/pdf/2611.05377v1)
