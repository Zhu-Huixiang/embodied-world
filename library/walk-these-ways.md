# Walk These Ways: Tuning Robot Control for Generalization with Multiplicity of Behavior

出处：CoRL 2022。研究范围：多步态四足控制与测试时调节。

[原文入口](https://proceedings.mlr.press/v205/margolis23a.html) · [原文 PDF](https://proceedings.mlr.press/v205/margolis23a/margolis23a.pdf) · [作者项目 / 代码入口](https://gmargo11.github.io/walk-these-ways/)

CoRL 2022；PMLR 205 论文集出版年为 2023。

阅读问题：**遇到新地面不重训，能否直接调一组步态参数让同一个策略换种走法？**

收录理由：将步态多样性组织成可操作控制接口，公开四足控制器和实际任务，具备明确复用价值与读者直观入口。

证据入口：可调参数定义清楚，有实机多行为、能耗和分布外任务比较，公开控制器使读者能够继续实验。

具身关联：将步态多样性组织成可操作控制接口，公开四足控制器和实际任务，具备明确复用价值与读者直观入口。

解读进度：候选选题。

元数据核对：2026-10-10；按原文、作者页或正式论文集记录。

[论文地图](../paper-map/README.md) · [刊会索引](../venues/README.md) · [首页](../README.md)

<!-- discovery:start -->
[机制简析、七维评分与雷达](../leaderboard/papers/walk-these-ways/README.md)

机制简析：一个策略同时接收三维速度命令和八维行为参数，后者控制足端相位、频率、身体姿态与抬脚等走法。历史本体观测与这些命令共同输入网络，输出十二个关节的位置目标。测试时人可以调整行为参数，在不重训情况下为新任务挑选合适步态。
<!-- discovery:end -->
