# VLA Paper Watch

自动追踪 Vision-Language-Action（VLA）、具身智能与机器人操作领域的近期高质量论文。仓库仅保存原创中文简介、元数据和原始论文链接，不保存论文 PDF。

## 论文索引

| 收录日期 | 论文 | 来源 | 链接 | 一句话简介 |
| --- | --- | --- | --- | --- |
| 2026-11-05 | MESA: An Evaluation Framework for Compositional, Semantic, and Spatial Generalization in Robotics | CoRL 2026 / arXiv | [arXiv:2611.05567](https://arxiv.org/abs/2611.05567) · [简介](papers/2026-11-05/mesa-generalization-benchmark.md) | 以单臂和双臂任务诊断机器人策略的空间、物体类别与组合泛化。 |
| 2026-11-05 | ELA: End-to-End Latent Action Policy Learning from Video Demonstrations | CoRL 2026 / arXiv | [arXiv:2611.05571](https://arxiv.org/abs/2611.05571) · [简介](papers/2026-11-05/ela-latent-action-policy.md) | 联合学习视频潜在动作、策略与动作解码器，减少机器人示范需求。 |
| 2026-11-05 | A³-VLA: Automatic Perception-Guided Attention Alignment for Robot Manipulation | NeurIPS 2026 / arXiv | [arXiv:2611.06447](https://arxiv.org/abs/2611.06447) · [简介](papers/2026-11-05/a3-vla-attention-alignment.md) | 用自动提取的交互区域监督 VLA 注意力，提高操作任务成功率。 |
| 2026-11-05 | Reinforcement Learning Enables Scaling Generalist Robot Policy Improvement | arXiv 预印本 | [arXiv:2611.06905](https://arxiv.org/abs/2611.06905) · [简介](papers/2026-11-05/generalist-robot-rl-improvement.md) | 扩大在线训练任务的覆盖与动作多样性，促进通用策略向未见任务迁移。 |
| 2026-11-05 | LoopQ: Fair, Closed-Loop Evaluation of Quantized Vision-Language-Action Models | arXiv 预印本 | [arXiv:2611.05093](https://arxiv.org/abs/2611.05093) · [简介](papers/2026-11-05/loopq-vla-quantization-benchmark.md) | 通过统一闭环基准衡量 VLA 量化的成功率、显存与实际时延。 |
| 2026-11-05 | Human-to-Robot Transfer via Bridging Representation and Action Space in VLAs | CoRL 2026 Workshop / arXiv | [arXiv:2611.04391](https://arxiv.org/abs/2611.04391) · [简介](papers/2026-11-05/h2rb-human-to-robot-transfer.md) | 以几何表征对齐和共享潜在动作将无配对人类示范迁移到机器人 VLA。 |
| 2026-11-05 | Asynchronous Robot Policies | arXiv 预印本 | [arXiv:2611.05155](https://arxiv.org/abs/2611.05155) · [简介](papers/2026-11-05/asynchronous-robot-policies.md) | 用低频语义记忆与高频动作专家解耦 VLA 的推理时延和机器人反应速度。 |
| 2026-11-05 | RoboTryOn: Synthesizing Dexterous Robot Demonstrations from Human Videos via Virtual Try-On | arXiv 预印本 | [arXiv:2611.05163](https://arxiv.org/abs/2611.05163) · [简介](papers/2026-11-05/robotryon-human-video-demonstrations.md) | 将人类视频合成为目标机器人视频与动作标签，扩展灵巧操作训练数据。 |
| 2026-11-05 | FloMo: 3D Scene Flow as a World Action Model Intermediate for Learning from Human Video | arXiv 预印本 | [arXiv:2611.05062](https://arxiv.org/abs/2611.05062) · [简介](papers/2026-11-05/flomo-scene-flow-world-action.md) | 以三维场景流承接人类视频运动先验，改善世界动作模型的操作泛化。 |
| 2026-11-05 | DreamX: Video Diffusion Model is a Universal Latent Action Learner | arXiv 预印本 | [arXiv:2611.05377](https://arxiv.org/abs/2611.05377) · [简介](papers/2026-11-05/dreamx-latent-action.md) | 从视频扩散模型抽取跨具身的紧凑潜在动作，支持人到机器人迁移。 |
| 2026-11-05 | Action Intent as a Bridge: Transferring Manipulation Knowledge from Human-Centric Videos to Robots | arXiv 预印本 | [arXiv:2611.04522](https://arxiv.org/abs/2611.04522) | 通过显式与隐式“动作意图”把人类视频中的操作知识迁移给机器人 VLA。 |

## 目录约定

- `papers/YYYY-MM-DD/`：每篇论文的中文简介。
- `data/papers.json`：用于去重的结构化索引；以 arXiv ID、DOI、标题和 URL 交叉去重。
