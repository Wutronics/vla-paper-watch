# DreamX: Video Diffusion Model is a Universal Latent Action Learner

## 基本信息

- **作者**：Jisoo Kim、Chaehyun Kim、Junsu Kim、Jiho Park、Seongchan Kim、Eunbeen Hong、Soowon Son、Fu-En Yang、Seungryong Kim
- **首次公开**：2026-11-03
- **会议/状态**：arXiv 预印本（arXiv:2611.05377）
- **论文**：[arXiv 摘要页](https://arxiv.org/abs/2611.05377)
- **项目页**：[DreamX](https://cvlab-kaist.github.io/DreamX/)
- **代码**：项目页标注待发布，暂无可核实仓库链接。

## 研究问题
从视频学习的潜在动作常混入视角、外观和具身差异，导致同一动作在不同人、机器人和环境之间难以共享。

## 核心方法
DreamX 复用预训练视频扩散模型的时空特征和生成先验，用可学习查询把每帧 1200 个视频潜在 token 压缩为 4 个动作 token；解码器根据首帧和动作 token 重建未来，让潜在变量更集中表达运动而非外观。

## 实验任务与主要结果
在 LARYBench，潜在动作的平均回归误差为 0.17，最强比较基线 DiLA 为 0.38；平均动作分类准确率为 69.67%，DiLA 为 62.25%。HumanAndRobot 零样本人到机器人视频迁移的 FVD 为 57.44，比较基线 AdaWorld 为 170.19。项目页还展示双臂机器人上的开环动作迁移，但该部分主要为定性展示。

## 对 VLA 的价值
提供跨人类与机器人形态复用的紧凑动作接口，可把无动作标签视频的运动先验迁移给动作生成策略，减少直接建模完整视频的计算量。

## 局限或待验证点
代码尚未公开；真实机器人迁移展示为开环且主要是定性结果。潜在动作基准与闭环任务成功率并非同一指标，仍需验证其在复杂长程 VLA 控制中的收益。

## 核验来源

- [arXiv 官方摘要页](https://arxiv.org/abs/2611.05377)
- [作者项目页及实验表](https://cvlab-kaist.github.io/DreamX/)
