# Stochastic Self-Distillation for Flow-Based Vision-Language-Action Models

- **作者**：Jingru Guo、Alessandra Russo、Joey Bose、Christos Ziakas
- **首次公开**：2026-11-16；**状态**：arXiv 预印本
- **论文**：[arXiv](https://arxiv.org/abs/2611.20460)；**项目页/代码**：官方摘要未提供可核实链接。

## 研究问题
流匹配 VLA 在线强化学习时，每次采样需要多步 ODE 积分且候选动作多样性不足，使分组奖励优化成本高、效果受限。

## 核心方法
VLA-SSD 将预训练动作头自蒸馏成由布朗路径条件化的随机单步生成器，并推导动作密度，支持基于似然比的强化学习后训练。

## 实验任务与主要结果
从 π0 蒸馏后，动作头前向耗时降低 7.7 倍，代价是 LIBERO 成功率相对下降 5.5%；利用更丰富的候选组对 π0.5 进行 GRPO 后训练，作者报告相对提升 20.6%。

## 对 VLA 的价值
把快速采样和随机探索引入流式 VLA，为高成本在线后训练提供更实用的动作生成接口。

## 局限或待验证点
单步蒸馏本身损失部分模仿性能；摘要未说明真实机器人效果和完整系统吞吐，需区分动作头加速与端到端加速。

**核验来源**：[arXiv 官方摘要](https://arxiv.org/abs/2611.20460)。
