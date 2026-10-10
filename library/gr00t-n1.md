# GR00T N1: An Open Foundation Model for Generalist Humanoid Robots

出处：arXiv 2025。研究范围：跨本体VLA与实机双臂操作、人类/仿真/生成轨迹混合训练。

[原文入口](https://arxiv.org/abs/2503.14734) · [原文 PDF](https://arxiv.org/pdf/2503.14734v2) · [作者项目 / 代码入口](https://github.com/NVIDIA/Isaac-GR00T)

原研究2503.14734，不以N1.5/N1.6/N1.7各建一篇。官方研究记录为ArXiv Preprint；预印本初次上传2025-03-18，不误用页面研究发布日03-17或v2更新03-27作为首投日期。

阅读问题：**Eagle-2视觉语言特征与连续动作流怎样分工，合成视频里的动作标签从哪来，预训练收益又在什么任务上成立？**

收录理由：开源机器人foundation model体系的重要原研究，供后续N1.X与人类数据工作建立机制前置；正式精讲队列仍待有正式刊会身份。

证据入口：H=16 action chunk；224×224 frame经pixel shuffle得64image tokens；N1-2B取Eagle-2第12层；K=4flow matching步；robot state/action由每本体MLP接通共享embedding。（§2.1 / Fig3）；in-house88小时teleop扩为827小时neural videos；DexMimicGen780000模拟轨迹≈6500小时。无动作视频经LAPA/IDM伪label，不能把生成时长当真实示范小时。（§2.2/§3 and Fig1/5）；100demos/task的RoboCasa/DexMG/GR-1平均：N1-2B32.1/66.5/50.0，总45.0%；Diffusion Policy25.6/56.1/32.7，总33.4%。（§4.4/Table2）

具身关联：跨本体VLA与实机双臂操作、人类/仿真/生成轨迹混合训练；Eagle-2视觉语言特征与连续动作流怎样分工，合成视频里的动作标签从哪来，预训练收益又在什么任务上成立？

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/gr00t-n1/README.md)

机制简析：Eagle-2视觉语言middle-layer tokens→DiT交叉注意力；embodiment-specific MLP编码state与noisy action、解码H=16连续动作块，flow-matching训练、K=4步采样。人类latent-action、real robot、DexMimicGen模拟和生成视频IDM/LAPA伪动作组成数据金字塔。
<!-- discovery:end -->
