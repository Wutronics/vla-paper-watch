# FloMo: 3D Scene Flow as a World Action Model Intermediate for Learning from Human Video

## 基本信息

- **作者**：Jeremy Collins、Namra Patel、Ayush Agarwal、Shitij Govil、Animesh Garg
- **首次公开**：2026-11-03；2026-11-04 发布修订版
- **会议/状态**：arXiv 预印本（arXiv:2611.05062）
- **论文**：[arXiv 摘要页](https://arxiv.org/abs/2611.05062)
- **项目页**：[FloMo](https://flomo-wam.github.io/)
- **代码**：[pairlab/flomo](https://github.com/pairlab/flomo)

## 研究问题
以未来 RGB 视频训练世界动作模型会消耗容量去预测外观细节；这些细节未必帮助机器人推断可执行动作，人类视频中的运动知识也难以直接迁移。

## 核心方法
FloMo 将三维场景流渲染为 RGB 并送入预训练视频模型的潜在空间，微调 5B 视频生成骨干联合预测三维运动和动作 token。训练混合无动作标签的人类视频与有动作标签的机器人遥操作数据，随后只用机器人数据细化动作预测。

## 实验任务与主要结果
真实双臂机器人三项分布内任务平均成功率为 91%，对应视频加运动目标的 51% 和仅视频目标的 40%。三项分布外任务共 30 次执行，FloMo 成功 18 次，DreamZero 与 AMPLIFY 各 6 次；移除人类视频后，在较小的 15 次评估中仅成功 1 次。RoboTwin 五项仿真任务平均成功率 63.6%，高于 π0.5 的 44.8% 和 FAST-WAM 的 41.0%。

## 对 VLA 的价值
把三维运动作为人类视频预训练与机器人动作之间的中间表示，为 VLA/WAM 选择预测目标提供了可测量的证据，并展示无标签人类视频对未见任务的贡献。

## 局限或待验证点
依赖场景流估计与较大的 5B 骨干；真实机器人分布外评估只有每任务 10 次，移除人类视频的消融每任务 5 次。跨平台及更长任务的收益仍需验证。

## 核验来源

- [arXiv 官方摘要页](https://arxiv.org/abs/2611.05062)
- [作者项目页及实验表](https://flomo-wam.github.io/)
