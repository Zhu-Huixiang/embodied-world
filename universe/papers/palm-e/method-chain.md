# 本篇方法链路 · PaLM-E

视觉和连续状态由编码器变成与语言 token 等维的向量，和文本交错组成多模态句子，再交给 decoder-only 语言模型生成文字。训练同时覆盖机器人任务、视觉问答和图文任务，以检验知识是否产生正迁移。机器人演示中，文字计划交给底层策略执行，后续视觉反馈再进入模型。

视觉和连续状态由编码器变成与语言 token 等维的向量，和文本交错组成多模态句子，再交给 decoder-only 语言模型生成文字。训练同时覆盖机器人任务、视觉问答和图文任务，以检验知识是否产生正迁移。机器人演示中，文字计划交给底层策略执行，后续视觉反馈再进入模型。

[本篇星系](../palm-e.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/palm-e.md) · [原文依据](https://proceedings.mlr.press/v202/driess23a.html)
