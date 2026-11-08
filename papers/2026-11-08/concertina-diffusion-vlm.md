# Concertina: Embodying Manipulation and Cognition in One Diffusion Vision-Language Model

- **作者**：Chengcheng Wang、Wei He、Wenhao Li、Hongguang Li、Kai Han、Jianyuan Guo、Chang Xu
- **首次公开**：2026-11-05；**状态**：arXiv 预印本
- **论文**：[arXiv](https://arxiv.org/abs/2611.07513)；**代码**：[GitHub](https://github.com/lose4578/Concertina)；**项目页**：未核实到独立项目页。

## 研究问题
常见 VLA 把动作离散化，或另接动作专家；这使连续轨迹的物理意义、认知与控制之间的共同训练变得困难。

## 核心方法
将每个控制时刻表示为共享扩散视觉语言骨干中的连续潜在动作 token，以相同的噪声重建算子生成动作块，并在物理坐标上监督。动作专属投影只占 4.46B 模型参数的 0.21%，没有独立动作专家层。

## 实验任务与主要结果
作者报告常规 LIBERO 平均成功率 98.15%，10,030 任务的 LIBERO-Plus 为 85.9%，CALVIN ABC-D 平均完成链长 4.142；代码仓库提供训练、检查点和评估流程。

## 对 VLA 的价值
给出把连续动作生成直接置于共享视觉语言模型中的架构和可复现实现，可用于研究统一表征是否优于分离动作头。

## 局限或待验证点
摘要中的成绩以作者实验为准；大模型推理成本、真实机器人闭环效果及其他具身平台上的泛化仍需验证。

**核验来源**：[arXiv 官方摘要](https://arxiv.org/abs/2611.07513)、[作者代码仓库](https://github.com/lose4578/Concertina)。
