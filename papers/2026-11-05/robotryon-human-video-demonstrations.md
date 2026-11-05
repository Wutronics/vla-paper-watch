# RoboTryOn: Synthesizing Dexterous Robot Demonstrations from Human Videos via Virtual Try-On

## 基本信息

- **作者**：Seungyong Lee、Suhyeok Jang、Minyoung Kim、Jinwoo Shin
- **首次公开**：2026-11-03；2026-11-04 发布修订版
- **会议/状态**：arXiv 预印本（arXiv:2611.05163）
- **论文**：[arXiv 摘要页](https://arxiv.org/abs/2611.05163)
- **项目页**：[RoboTryOn](https://ryan-seungyong-lee.github.io/RoboTryOn/)
- **代码**：[RoboTryOn](https://github.com/ryan-seungyong-lee/RoboTryOn)

## 研究问题
人类第一人称视频可低成本收集，但直接叠加机器人外观或将人手姿态重定向为机械手动作，会留下视觉与动作差距，尤其影响高自由度和双臂操作。

## 核心方法
RoboTryOn 将人转为目标机器人视作“虚拟试穿”：根据机器人参考图和手部骨架逐步转换关键帧，合成保留任务、物体与背景的机器人视频，再用结合深度特征的逆动力学模型估计动作标签，训练机器人策略。

## 实验任务与主要结果
在 OpenArm、RB-Y1 等形态的七项无目标任务遥操作示范的任务上，作者报告平均成功率从 2% 提升至 60%。项目页给出的两个机器人分布外任务成功率分别为 73.0% 和 46.9%，单用遥操作数据为 3.1% 和 1.0%；评估按每任务 28 次试验统计。作者还称，以约三分之一的数据收集成本可匹配仅用遥操作训练的策略。

## 对 VLA 的价值
把可扩展的人类视频转成带视觉和动作标签的目标机器人演示，为 VLA 的新任务适配提供数据生成路径，覆盖灵巧手与双臂任务。

## 局限或待验证点
结果依赖视频生成质量、机器人外观匹配和逆动力学动作标注；跨更多相机视角、物体交互与长时任务的鲁棒性仍需验证。成本比较也需结合具体硬件与生成开销理解。

## 核验来源

- [arXiv 官方摘要页](https://arxiv.org/abs/2611.05163)
- [作者项目页及实验表](https://ryan-seungyong-lee.github.io/RoboTryOn/)
