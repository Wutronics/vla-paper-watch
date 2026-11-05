# Reinforcement Learning Enables Scaling Generalist Robot Policy Improvement

## 基本信息

- **作者**：Michal Korniak、Marco Bagatella、Ralf Römer、Michal Nauman、Yarden As、Pranav Vignesh、Manan Agarwal、Leander Diaz-Bone、Piotr Zalewski、Mikołaj Czarnecki、Lenart Treven、Shashwat Saxena、Sreyas Venkataraman、Sarvesh Patil、Zhiyuan Zhou、Daniel Marta、Oier Mees、Nur Muhammad Mahi Shafiullah、Carmelo Sferrazza、Bhavya Sukhija、Angela P. Schoellig、Andreas Krause、Max Simchowitz、Andrew Wagenmaker
- **首次公开**：2026-11-04
- **会议/状态**：arXiv 预印本；作者项目页注明已投稿 ICLR 2027，尚非录用
- **论文**：[arXiv 摘要页](https://arxiv.org/abs/2611.06905)
- **项目页**：[Generalist Improvement](https://lasgroup.github.io/generalist-improvement/)
- **代码**：[lasgroup/generalist-improvement](https://github.com/lasgroup/generalist-improvement)

## 研究问题
通用机器人策略在线强化学习后常只改善单一部署任务，并可能遗忘其他能力。研究要判断能否同时改进多任务，并把收益推广到在线训练未见过的任务。

## 核心方法
论文设计训练任务、未见场景和未见物体的分离评估，比较成功轨迹过滤微调、价值函数引导的候选动作筛选（BoN）和价值函数引导的策略提取（OGPO），并系统改变在线训练任务的数量与多样性。

## 实验任务与主要结果
在 MolmoSpaces 中，作者将训练任务从 1 扩展至 144，并在未见场景和物体上测试；同时在 LIBERO 检查未见任务。结果表明，多任务覆盖足够广时，BoN 与 OGPO 可从单任务训练常见的遗忘转向对未见设置的性能提升；价值函数方法的泛化通常优于只过滤成功轨迹的微调。作者尤其发现训练任务所需动作策略的多样性会影响迁移范围。

## 对 VLA 的价值
为通用 VLA 的部署后持续改进提供评估框架和强化学习配方，指出提升训练任务成功率不等于保住或扩展原有泛化能力。

## 局限或待验证点
主要证据来自仿真基准；真实机器人在线多任务改进及采样成本尚需验证。作者项目页的部分增益数值仍是占位符，因此本简介不引用这些未定量值。

## 核验来源

- [arXiv 官方摘要与 HTML 原文](https://arxiv.org/abs/2611.06905)
- [作者项目页](https://lasgroup.github.io/generalist-improvement/)
