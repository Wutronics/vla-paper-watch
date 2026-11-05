# MESA: An Evaluation Framework for Compositional, Semantic, and Spatial Generalization in Robotics

## 基本信息

- **作者**：Albert Wilcox、Frank Chang、Nhi Nguyen、Aishani Chakraborty、Jeremy A. Collins、Vaibhav Saxena、Benjamin Joffe、Siddharth Karamcheti、Animesh Garg
- **arXiv 发布日期**：2026-11-03
- **会议/状态**：CoRL 2026 会议论文；本次为上次成功运行后新发现
- **论文**：[arXiv 摘要页](https://arxiv.org/abs/2611.05567)
- **项目页**：[MESA](https://www.pair.toronto.edu/MESA/)
- **代码**：[pairlab/mesa-env](https://github.com/pairlab/mesa-env)

## 研究问题
现有机器人操作基准有的已接近饱和，有的无法控制分布变化，难以区分语言条件策略究竟能否泛化到新位置、新物体与新任务组合。

## 核心方法
MESA 提供分布内评估及四个分布外维度：空间配置、物体实例、物体类别和子任务组合。MESA-Gen 扩展 MimicGen 以生成任务与示范；单臂 MESA 与双臂 BiMESA 均提供训练集和五套评估集。

## 实验任务与主要结果
作者在单臂桌面操作与双臂协调任务上比较七类策略，包括扩散策略、基于 VLM 的方法及预训练 VLA。最强模型在 MESA 的平均成功率为 52.0%，在 BiMESA 为 48.7%；未知物体类别与组合任务尤其困难。项目页还显示某些预训练收益在双臂设置中并不稳定。

## 对 VLA 的价值
提供可控的语言、空间和开放词汇泛化诊断，便于评价 VLA 在真实操作中常见的分布偏移，而不只比较单一平均成功率。

## 局限或待验证点
基准主要在仿真桌面操作中评估，榜单与真实机器人表现的一致性仍需更多平台验证；任务生成与训练数据分布也可能影响模型排名。

## 核验来源

- [arXiv 官方摘要页](https://arxiv.org/abs/2611.05567)
- [作者项目页与结果表](https://www.pair.toronto.edu/MESA/)
