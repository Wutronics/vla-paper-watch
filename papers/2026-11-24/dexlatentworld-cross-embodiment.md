# DexLatentWorld: 3D Cross-Embodiment Latent Action World Models for Zero-Shot Robotic Manipulation

- **作者与机构**：Vinay Udit Mohan、Xuchuan Huang、Rolandos Alexandros Potamias；Imperial College London
- **首次公开**：2026-11-23；**状态**：arXiv 预印本，未核实正式录用
- **论文**：[arXiv](https://arxiv.org/abs/2611.30907)；**项目页**：[DexLatentWorld](https://vinaymohan0409.github.io/DexLatentWorld/)；**代码**：[GitHub](https://github.com/VinayMohan0409/DexLatentWorld)。

## 研究问题
世界模型依赖昂贵的动作标注，且动作空间通常绑定训练时的机器人形态，难以迁移到未见过的灵巧手。

## 核心方法
从重定向到多种机器人手的人类操作点云中学习连续潜在动作；跨形态对比损失对齐同一运动的表示。预测每个三维点的未来位移，在潜在空间做模型预测控制，并由几何运动恢复可执行命令，无需每种机器人专属的动作解码器。

## 实验与主要结果
项目页报告训练涉及人类和八种机器人手、约 4.1 万个转移。任务无关适配后，伸手、抓取、放置成功率为 90%、92%、60%，对照 DexWM 报告值为 72%、58%、28%；未见过的真实灵巧手在五项任务的 50 次试验中成功率 86%。论文和代码提供潜在动作、规划方式等对照；与 DexWM 的部分数字来自对方报告，需注意协议一致性。

## 研究价值
为跨形态机器人学习建立几何驱动的潜在动作接口，对减少形态专属标注与策略重训有研究价值。

## 局限与待验证点
依赖点云质量、已知几何与运动学；真机样本仍限于一套未见手及五项任务。代码已公开，但仓库说明训练检查点尚待另行发布。

## 综合质量评价
- **AI 综合评分**：87/100（创新 23/25；实验 21/25；研究价值 19/20；真机与泛化 17/20；可复现性 7/10）。
- **依据与推荐**：跨形态潜在动作、未见手真机结果和公开代码构成较强证据；检查点未发布。**阅读优先级：推荐**。

**核验来源**：[arXiv 官方摘要](https://arxiv.org/abs/2611.30907)、[作者项目页](https://vinaymohan0409.github.io/DexLatentWorld/)、[代码仓库](https://github.com/VinayMohan0409/DexLatentWorld)。评分为 AI 辅助判断，并非官方评级。
