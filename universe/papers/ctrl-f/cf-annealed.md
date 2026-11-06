# 在自己走到的状态学教师，再用奖励修正 · Ctrl-F

PPO训练同时加入逐渐减弱的教师模仿损失。

解析教师在当前策略访问状态上给目标，类似DAgger；模仿权重按DAPG思路衰减。奖励评估物体参考跟踪，低层冻结。论文未列完整损失权重、网络宽度和训练预算。

继续拆：[模仿力指令，可能仍没把力传给物体](cf-bc-rl.md) · [去掉教师的证据是定性观察](cf-rl-only.md)。

[本篇星系](../ctrl-f.md) · [论文解读/导读](https://github.com/Zhu-Huixiang/embodied-world/blob/main/library/ctrl-f.md) · [原文依据](https://arxiv.org/pdf/2611.05507v1)
