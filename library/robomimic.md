# What Matters in Learning from Offline Human Demonstrations for Robot Manipulation

出处：CoRL 2021。研究范围：离线人类示范学习的系统对照与 robomimic 工具基础。

[原文入口](https://proceedings.mlr.press/v164/mandlekar22a.html) · [原文 PDF](https://proceedings.mlr.press/v164/mandlekar22a/mandlekar22a.pdf) · [作者项目 / 代码入口](https://arise-initiative.github.io/robomimic-web/)

CoRL 2021 主会在五年窗内；PMLR 2022。首公开早于窗口，作为模仿学习基线基础记录。项目网页此次 Exa 抓取为空，方法核验使用正式 PDF。

阅读问题：**同样的人类示范，为什么换个观测历史、数据质量或停训方式，结果会差这么多？**

收录理由：robomimic 生态的原始系统研究，澄清人类数据下行为克隆、离线 RL 和历史观测的差异，基础价值高。

证据入口：正式 PDF 给出六类算法、仿真/真实多阶段任务、多随机种子及示范质量研究，开源数据与统一实现支撑公平对照；系统证据价值高于单个新网络模块。

具身关联：robomimic 生态的原始系统研究，澄清人类数据下行为克隆、离线 RL 和历史观测的差异，基础价值高。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/robomimic/README.md)

机制简析：同一组操作任务上更换算法、单人或多人示范、低维或图像观测，并控制训练和评估流程，观察各因素独立造成的差异。带历史的行为克隆能处理人类动作的时序相关性；离线 RL 在机器生成数据上的表现不能直接搬到人类数据。它还检验验证损失与执行成功率不一致时，选模型会发生什么。
<!-- discovery:end -->
