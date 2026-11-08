# AffectiveVLA: Safe and Intent-Aware VLA Control for Human-Humanoid Social Interaction

- **作者**：Nikita Kuzmin、Georgii Demianchuk、Mariya Lezina、Yara Mahmoud、Iana Zhura、Miguel Altamirano Cabrera、Dzmitry Tsetserukou
- **首次公开**：2026-11-05；**状态**：arXiv 预印本
- **论文**：[arXiv](https://arxiv.org/abs/2611.07712)；**项目页/代码**：官方摘要未提供可核实链接。

## 研究问题
握手、碰拳和拥抱要求人形机器人先识别人类意图，再进行安全、实时的接触动作；直接执行 VLA 输出易误触发。

## 核心方法
两台机载相机的 RGB 意图识别器为 VLA 生成语言提示，低置信度时抑制动作；接触阶段使用交互专属柔顺控制，并有独立的语音触发安全停止。

## 实验任务与主要结果
作者采集约 1,300 条 VR 遥操作多模态交互轨迹，微调四种 VLA，并在 Unitree G1 人形机器人上评估。独立模型中 GR00T 最佳；加入意图识别后，系统 macro-F1 从 0.75 提升到 0.90，意图模型 p95 推理延迟 6.27 毫秒。

## 对 VLA 的价值
展示 VLA 在真实人机接触中的系统集成方式，把意图门控、柔顺控制和安全停止纳入闭环执行。

## 局限或待验证点
结果集中于单一人形平台与少数社交接触任务；跨人群、复杂干扰及长期安全性仍需验证。

**核验来源**：[arXiv 官方摘要](https://arxiv.org/abs/2611.07712)。
