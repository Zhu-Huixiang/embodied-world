# 4.1 先把评测的单位讲清楚 · Holo-M

generalist 一个 checkpoint，在 SIMPLE 的 24 个任务上联合训练，评估六个代表任务。每项三个随机化等级，每格十次，6×3×10=180。specialist 则按任务分别适配。前者问“一个模型能顾几摊事”，后者问“专练这一摊能到哪儿”。<!-- evidence:C11 -->

generalist 一个 checkpoint，在 SIMPLE 的 24 个任务上联合训练，评估六个代表任务。每项三个随机化等级，每格十次，6×3×10=180。specialist 则按任务分别适配。前者问“一个模型能顾几摊事”，后者问“专练这一摊能到哪儿”。 checkpoint 是保存下来的模型参数，像一个可继续训练、也可拿来测试的存档。随机化等级改变任务条件，下面总分和难格子要一起看。

[在完整解读里看计算与例子](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/holo-m-2609.35709/README.md#41-先把评测的单位讲清楚)

[本篇星系](../holo-m.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/articles/holo-m-2609.35709/README.md) · [原文依据](https://arxiv.org/abs/2609.35709)
