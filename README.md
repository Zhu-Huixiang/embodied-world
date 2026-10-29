<h1 align="center">具身智能的 World</h1>

<p align="center"><strong>从论文里的一个问题，走到机器人实际计算的那一步</strong></p>

这里与同名公众号一起读具身智能论文。每篇先交代技术分歧，提出三个问题，再沿原文目录拆输入、表示、公式、训练信号与闭环实验。公众号适合顺着主线阅读；GitHub 留下高清图、公式源文件、证据位置和继续读的入口。

## 七个入口

| 功能 | 从这里开始 | 能找到什么 |
| --- | --- | --- |
| 论文解读 | [已完成稿件](#论文解读) | 原创中文解读、论文原图、公式与 DrawPaper 图源 |
| 具身论文地图 | [研究问题与阅读路线](paper-map/README.md) | 按问题组织世界模型、WAM、视频动作、VLA、RL、操作、感知与运动控制 |
| 顶会顶刊集锦 | [按正式出处查论文](venues/README.md) | 常用简称、领域定位、CCF/影响因子/分区科普与正式论文入口 |
| 解读日程 | [未来一周的拟定选题](calendar/README.md) | 每天准备细讲哪篇、带着什么问题读、当前进度 |
| arXiv 新作集锦 | [按日期追论文](arxiv/README.md) | 带首投/收录时间与已核实机构；重点实验室与具体研究贡献一起筛 |
| 具身榜 | [七维阅读优先榜](leaderboard/README.md) · [交互筛选榜](https://zhu-huixiang.github.io/embodied-world/leaderboard/) · [作者与团队](leaderboard/origins/README.md) | 每篇机制简析、雷达、引用与跨平台信号；按八列组合筛选和排序，沿作者、实验室与大学继续读相关工作 |

| 知识点宇宙 | [论文与知识点图谱](universe/README.md) · [交互宇宙](https://zhu-huixiang.github.io/embodied-world/universe/) | 从论文到方法、模块和共享技术；已精讲的节点点亮，可沿关联查讲解与使用它的论文 |

正式公众号精讲按具身榜顺序推进，优先影响力与证据扎实的论文。Holo-M 是试水稿。[高影响论文清单与收录理由](paper-map/curated-2026-10-10.md)列出正式出处、具身关联和经典破例理由；[完整精讲队列](calendar/queue.md)随榜单更新。[补查与收录决定](leaderboard/selection-2026-10-10.md)记录近期新加入、正式出处更新和暂缓项。

## 论文解读

- [ACT：机器人别再一步一猜，先把一段动作想明白](articles/act-2304.13705/README.md)
- [Transformer：句子不排队读了，意思还接得上吗？](articles/attention-1706.03762/README.md)
- [CLIP：把分类器写成一句话，凭什么管用？](articles/clip-2103.00020/README.md)
- [DDPM：只学预测噪声，怎么就能画画了？](articles/ddpm-2006.11239/README.md)
- [Diffusion Policy：动作也能靠去噪生成？](articles/diffusion-policy-2303.04137/README.md)
- [DINO：没人教它认狗，注意力却把狗圈了出来？](articles/dino-2104.14294/README.md)
- [DiT：扩散画图，非得长一张 U-Net 的脸吗？](articles/dit-2212.09748/README.md)
- [DreamerV3：脑内练习，怎么没练成“幻想高手”？](articles/dreamerv3-2301.04104/README.md)
- [3DGS：不用沿光线慢慢找，撒一把椭球就能画？](articles/gaussian-splatting-2308.04079/README.md)
- [全身动作写成208个token，机器人就懂了吗？](articles/holo-m-2609.35709/README.md)
- [LDM：画一张大图，为什么先把战场缩小？](articles/latent-diffusion-2112.10752/README.md)
- [MAE：把图遮掉四分之三，为什么反而学会了看？](articles/mae-2111.06377/README.md)
- [MuZero：不画出未来，怎么在脑内做规划？](articles/muzero-1911.08265/README.md)
- [NeRF：把照片藏进函数里，换个角度还能看见吗？](articles/nerf-2003.08934/README.md)
- [RT-1：机器人看过十三万次示范，就会举一反三了？](articles/rt1-2212.06817/README.md)
- [SAM：点一下就能抠图，它真知道你想要什么吗？](articles/sam-2304.02643/README.md)
- [SAM 2：点一下就一直跟住？视频分割最难的，其实是别失忆](articles/sam2-2408.00714/README.md)
- [ViT：把图片切碎，怎么就打过了卷积？](articles/vit-2010.11929/README.md)

公众号文章链接在公开发表后加入各篇页面。Holo-M 目前可读 GitHub 全稿，公众号稿仍待质量评阅与后台发表。

## 已完成解读的方向索引

- [世界模型](directions/world-model.md)（4 篇）
- [世界动作模型](directions/world-action-model.md)（0 篇）
- [视频动作模型](directions/video-action.md)（0 篇）
- [视频生成](directions/video-generation.md)（2 篇）
- [VLA](directions/vla.md)（5 篇）
- [强化学习](directions/reinforcement-learning.md)（2 篇）
- [运动控制与 Locomotion](directions/locomotion.md)（1 篇）
- [Manipulation](directions/manipulation.md)（4 篇）
- [Diffusion / Transformer](directions/diffusion-transformer.md)（9 篇）

## 一起读，也一起纠错

想看新稿，从[新作集锦](arxiv/README.md)进入；想挑下一篇，对照[具身榜](leaderboard/README.md)的理由和证据。想追一条路线，从[论文地图](paper-map/README.md)开始；想找正式原文，从[刊会集锦](venues/README.md)进入。若发现公式、数字或解释有问题，请在 Issues 留下原文位置，便于修订。

阅读和方法图工具：[ReadPaper skill](https://github.com/Zhu-Huixiang/ReadPaper/tree/main/readpaper) · [DrawPaper skill](https://github.com/Zhu-Huixiang/ReadPaper/tree/main/drawpaper)。

配套公众号：**具身智能的 World**。GitHub 保存关注入口，公众号底部“阅读原文”返回本篇解读。

![关注公众号：具身智能的 World](assets/wechat-qr.jpg)
