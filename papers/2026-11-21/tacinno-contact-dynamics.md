# TacInno: Teaching Vision-Language-Action Models the Contact Dynamics Beyond Vision and Action

- **作者**：Weile Li、Yunfan Lou、Muqing Shi、Zihao Zhang、Zhenbiao Huang、Boxian Yao、Xiyu Zhu、Zhibo Pang
- **首次公开**：2026-11-19；**会议/状态**：arXiv 预印本，未见官方会议录用信息
- **论文**：[arXiv](https://arxiv.org/abs/2611.26405)；**项目页**：[TacInno](https://tacinno.github.io/)；**代码**：[GitHub](https://github.com/LisavilaLee/TacInno)。

## 研究问题
在接触密集的操作中加入触觉输入后，VLA 有时仍忽视触觉，因为触觉变化的一部分可由图像和已执行动作预测。研究希望突出视觉与动作无法解释的接触信息。

## 核心方法
TacInno 把未来触觉变化中不可由视觉和动作解释的部分编码为离散“触觉创新”码。TacInno-VLA 在训练时预测该码作为辅助监督；部署时移除编码器和辅助预测头，保留触觉输入分支。

## 实验任务与主要结果
六项 UniVTAC 仿真任务平均成功率为 87.5%，四项真实任务为 70.5%，分别比最强视觉触觉对照高 10.7 和 9.0 个百分点。项目页的触觉关闭实验显示，在 Lift Can 任务上成功率从 88% 降至 0%，表明该策略确实依赖触觉输入。

## 对 VLA 的价值
给出了让触觉信息真正参与动作学习的训练信号设计，并提供可核查的代码与消融实验。

## 局限或待验证点
方法需要触觉传感器及其示范数据；所报告任务数量有限，跨传感器和跨机器人迁移仍待检验。

**核验来源**：[arXiv 官方摘要](https://arxiv.org/abs/2611.26405)、[作者项目页](https://tacinno.github.io/)、[官方代码仓库](https://github.com/LisavilaLee/TacInno)。
