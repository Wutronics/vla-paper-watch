# Human-to-Robot Transfer via Bridging Representation and Action Space in VLAs

## 基本信息

- **作者**：Junhyeong Park、Wook Jung、Taeyoung Kim、Huiwon Jang、Jinwoo Shin
- **首次公开**：2026-11-03
- **会议/状态**：CoRL 2026 Scaling H2R Workshop 口头报告；arXiv 预印本（arXiv:2611.04391）
- **论文**：[arXiv 摘要页](https://arxiv.org/abs/2611.04391)
- **项目页**：[H2RB](https://junhyeong-park.me/h2rb/)
- **代码**：[h2rb-code](https://github.com/jun-brro/h2rb-code)

## 研究问题
预训练 VLA 适配新机器人和新任务仍依赖昂贵的机器人示范。人类示范易收集，但视觉表征与动作空间都存在具身差异，直接混合训练难以迁移。

## 核心方法
H2RB 使用未配对的人类与机器人示范联合训练：以手腕和指尖几何锚定视觉表征，再用共享编码器和分别面向人、机器人的解码器学习共同的潜在动作空间，保留两种身体的运动特性。

## 实验任务与主要结果
在 OpenArm 的新物体抓取放置、开关空气炸锅及位置偏移任务上，作者报告物体迁移的加权任务分数从基线 8.0 提升到 51.8，技能迁移达到 62.7，分布外放置从 6.0 提升到 45.3。这里的 0–100 数值是执行进度加权分数，**不是成功率百分比**。RB-Y1 包裹任务的成功率为 78%，对比机器人单独训练的 64%。

## 对 VLA 的价值
同时对齐观察和动作两个接口，为从无配对人类示范扩展预训练 VLA 提供可执行路线，尤其适合目标任务缺少机器人演示的情形。

## 局限或待验证点
项目页的真实机器人评估集中于 OpenArm 和 RB-Y1；开源代码不含内部示范、校准数据与训练权重。跨更多机器人形态和未见场景的迁移仍待复现。

## 核验来源

- [arXiv 官方摘要页](https://arxiv.org/abs/2611.04391)
- [作者项目页及实验表](https://junhyeong-park.me/h2rb/)
