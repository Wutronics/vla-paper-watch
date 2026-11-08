# SLA: Scaling Spatial-Language-Action Model via Continual Pre-training

- **作者**：Fuhao Li、Wenxuan Song、Qizhou Huang、Ziyang Zhou、Jingbo Wang、Junwu E、Pengwei Wang、Yan Wang、Shunbo Zhou、Haoang Li
- **首次公开**：2026-11-05；**状态**：arXiv 预印本
- **论文**：[arXiv](https://arxiv.org/abs/2611.08373)；**代码**：[Spatial-Forcing/SLA](https://github.com/OpenHelix-Team/Spatial-Forcing/tree/master/SLA)（由 arXiv 摘要页提供）；**项目页**：arXiv 所列项目地址暂不可访问。

## 研究问题
二维视觉语言预训练难以赋予 VLA 可迁移的三维空间理解；只在任务微调时加入空间监督，可能限制跨任务和跨机器人泛化。

## 核心方法
以 π0.5 为基础，在持续预训练和下游微调中联合优化动作预测与视觉特征到冻结三维感知模型的空间对齐。特征门控汇聚多个网络层，并利用部分数据的深度和相机标定；训练时随机丢弃状态输入，推理时不增加空间教师或额外分支。

## 实验任务与主要结果
在 LIBERO-Plus、RoboTwin 2.0、RoboCasa-Panda、RoboDojo-Real 及八种真实部署条件测试。论文报告 LIBERO-Plus 总成功率 87.4%，RoboDojo-Real 为 33.9%（π0.5 为 12.8%）；八种真实部署条件平均 83.8%，比 π0.5 高 24.0 个百分点。

## 对 VLA 的价值
展示如何在基础模型持续预训练阶段注入三维空间监督，并保持原有推理结构，适用于跨具身、开放对象和动态场景研究。

## 局限或待验证点
预训练需要额外三维教师及异构数据清洗；部分基准任务和实体平台的增益差异较大，其他基础模型上仍需独立验证。

**核验来源**：[arXiv 官方摘要](https://arxiv.org/abs/2611.08373)、[论文 HTML 原文](https://arxiv.org/html/2611.08373v1)。
