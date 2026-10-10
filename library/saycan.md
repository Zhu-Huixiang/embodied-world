# Do As I Can, Not As I Say: Grounding Language in Robotic Affordances

出处：CoRL 2022。研究范围：语言模型规划、技能可供性与移动操作。

[原文入口](https://proceedings.mlr.press/v205/ichter23a.html) · [原文 PDF](https://proceedings.mlr.press/v205/ichter23a/ichter23a.pdf) · [作者项目 / 代码入口](https://say-can.github.io/)

CoRL 2022；PMLR 205 在 2023 年出版，不能按书目年份改成 CoRL 2023。

阅读问题：**语言模型觉得该做的事，机器人做得到吗？两个概率相乘到底解决什么？**

收录理由：把语言推理落到机器人实际技能能力上的代表路线，影响了后续 LLM 机器人规划与可供性约束研究。

证据入口：PMLR 正式论文与项目页给出真实厨房任务、语言模型替换、可供性约束实例及开源桌面版；创新是接口与组合机制，低层技能仍是独立预训练模块。

具身关联：把语言推理落到机器人实际技能能力上的代表路线，影响了后续 LLM 机器人规划与可供性约束研究。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/saycan/README.md)

机制简析：高层指令与已执行步骤送给语言模型，为每个候选技能估计它对任务的适用性；技能价值函数再估计当前场景下的执行成功可能。两者合并后选择技能、实际执行并把步骤加入上下文，直到选出结束。原文分开报告计划与执行，因而能看清语言推理和物理技能各自卡在哪里。
<!-- discovery:end -->
