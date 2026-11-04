# Compliant Residual DAgger: Improving Real-World Contact-Rich Manipulation with Human Corrections

**解读导读** · NeurIPS 2025 · [操作与动作块](../paper-map/README.md#track-manipulation)

研究范围：单套UR平台四项真实接触丰富操作；冻结基础策略、动觉在线纠正与力感知残差学习。

[原文入口](https://proceedings.nips.cc/paper_files/paper/2025/hash/cbf883a744952d4a40591271a58ab9d0-Abstract-Conference.html) · [原文 PDF](https://compliant-residual-dagger.github.io/files/CR_DAgger_extended.pdf) · [作者项目 / 代码入口](https://compliant-residual-dagger.github.io/) · [作者与团队](../leaderboard/origins/papers/cr-dagger.md)

研究首发于2025-06-20，NeurIPS2025主会原版为四作者、两任务。本次阅读官方项目提供的IJRR2026作者扩展稿（14页，加入Chendong Xin及齿轮插入/布线实验），期刊DOI为10.1177/02783649261498061；在线出版2026-11-02据出版社Crossref登记。原版与扩展版合为一篇研究，公开与评审沿已核NeurIPS阶段，不把期刊出版冒充本周新研究。

## 先看它做了什么

CR-DAgger保留低频扩散基策略，通过顺应式动觉接口在策略继续运行时采集人的位置增量和接触力纠正。扩展稿用参考速度跟踪和硬件时延对齐避免微小纠正标签被控制滞后淹没。冻结视觉编码器，力历史经时间卷积，与状态共同输入轻量残差头；残差推理循环约50Hz，每次预测5个间隔0.02s的15维动作（9维位姿表示与6维目标力/力矩），由500Hz导纳控制器执行基准动作加局部修正。无干预段学零残差，并对纠正附近数据重采样，避免用少量新数据直接改坏完整基策略。

## 带着什么问题读

**为什么人把机器人推回正确方向，训练出的策略反而会变差？纠正的采集方式、控制延迟和残差学习分别解决什么？**

## 为什么值得继续读

问题明确、接口可计算，四真实任务与同数据更新基线和关键消融支持机制。按同一研究身份首次入库；2026-11-02为此次发现的IJRR在线出版元数据事件，研究首发与扩展内容均非本周首次公开。

证据入口：作者扩展稿Fig9：四项实机任务分别20/32/20/20回合。翻书CR100%对原基策略40%，takeover版CR55%、on-policy无力残差35%；皮带96.8%对无力/带力基策略15.6%/43.8%、重训34.4%、微调0%、KL微调3.1%、无力残差28.1%；齿轮90%对5%/40%、重训50%、微调35%、KL25%、无力残差5%；布线100%对70%/25%、微调85%、KL95%、无力残差40%。Fig12翻书同50纠正数据一次训练100%，20+3×10分批最终0%；Fig13皮带1/2/3批90.6/96.8/87.5%，额外数据非单调。Fig12采样uniform70/dense-around75/dense-after100。AppendixA.4概率MLP100%、FlowTransformer90%各10回合，不能与主表32回合当等样本比较。未报告跨训练seed置信区间。

具身关联：直接连接人类在线干预、接触力反馈、模仿策略修正与机器人闭环控制。

全文精讲沿[编辑队列](../calendar/queue.md)推进；这里先保留方法主线与阅读问题。

[知识星系](../universe/papers/cr-dagger.md) · [七维评分与雷达](../leaderboard/papers/cr-dagger/README.md) · [NeurIPS集锦](../venues/NeurIPS/README.md) · [地图方向](../paper-map/README.md#track-manipulation) · [首页](../README.md)

元数据核对：2026-11-04。
