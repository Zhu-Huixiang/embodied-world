# 抓取矩阵连接接触力和物体力矩 · Ctrl-F

每个接触点三维力叠成f，抓取矩阵G把它映射到六维物体wrench。

目标是Gf≈W*且f属于可传力集合F，任务由(G,F,load)定义；正文称各分配可闭式批量求解，但没有逐通道闭式公式。n个接触时f为3n、G为6×3n，是由定义推得的维度。

[本篇星系](../ctrl-f.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/ctrl-f.md) · [原文依据](https://arxiv.org/pdf/2611.05507v1)
