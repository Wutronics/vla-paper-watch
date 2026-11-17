# Lift, See, Act: Hierarchical Robot Policy Pretraining with 3D Foundation Models

- **作者**：Yiyuan Ge、Changxing Ding、Ziyu Hao、Zijie Zheng、Xiangmin Xu
- **首次公开**：2026-11-16；**会议/状态**：NeurIPS 2026 接收论文
- **论文**：[arXiv](https://arxiv.org/abs/2611.20481)；**项目页**：[Lift, See, Act](https://yiyuan00.github.io/Lift-See-Act/)；**代码**：[GitHub](https://github.com/yiyuan00/Lift-See-Act)。

## 研究问题
从人类视频预训练机器人策略时，已有方法只保留稀疏三维手部轨迹，忽略三维基础模型在提取过程中产生的密集几何与交互信息。

## 核心方法
按 Lift、See、Act 三阶段预训练：把视觉浅层特征与多个三维模型的中间表征对齐，借深度图重建学习空间布局，并用手部区域引导注意力聚焦交互热点，再用于闭环机器人动作。

## 实验任务与主要结果
项目页报告 MetaWorld 消融平均成功率 92.2%，比不预训练高 18.9 个百分点；真实 Franka 六个条件平均成功率 68.3%，所列最强比较方法为 41.7%。达到基线峰值表现只需其 60% 的下游专家示范。

## 对 VLA 的价值
提供把无动作人类视频中的密集三维知识转化为机器人操作表征的分层训练方式。

## 局限或待验证点
依赖外部三维模型与手部检测质量；真实测试每条件仅 10 次，跨机器人平台和开放词汇指令能力尚需检验。

**核验来源**：[arXiv 官方摘要](https://arxiv.org/abs/2611.20481)、[作者项目页与结果表](https://yiyuan00.github.io/Lift-See-Act/)。
