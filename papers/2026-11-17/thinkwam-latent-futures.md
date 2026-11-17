# ThinkWAM: Rethinking Latent Futures for Action Refinement

- **作者**：Haoyun Tang、Baqiao Deng、Enjin Zhou、Songwen Tian、Keyao Xu、Bowen Jing、Kun Wang、Ke Ma、Zhandong Mei、Huibin Li
- **首次公开**：2026-11-16；**状态**：arXiv 预印本
- **论文**：[arXiv](https://arxiv.org/abs/2611.21258)；**项目页**：[ThinkWAM](https://thinkwam-project.github.io/)；**代码**：[GitHub](https://github.com/HaoyunT/Thinkwam)。

## 研究问题
世界动作模型的未来预测若不以拟执行动作作为条件，便不能反映该动作对场景的影响，限制执行前修正。

## 核心方法
采用“提出动作—重想未来—修正动作”的双遍流程：先产生完整动作块，再用它修正多时域未来潜变量，并将修正结果送入同一个动作头生成最终动作；加入可供性引导的观察动作记忆。

## 实验任务与主要结果
作者报告 LIBERO 成功率 98.70%、LIBERO-Plus 84.76%、RoboTwin 2.0 Clean/Random 85.75%/65.85%、RoboCasa24 65.17%，三种真实分布外条件平均 64.4%。双遍推理每动作块在 LIBERO 平均耗时 153.48 毫秒。

## 对 VLA 的价值
展示动作建议可在执行前主动修正潜在未来，再把反馈用于改进操作策略，而无需生成完整视频。

## 局限或待验证点
双遍动作头增加推理成本；不同硬件上的实时闭环效果及跨模型复现仍需验证。

**核验来源**：[arXiv 官方摘要](https://arxiv.org/abs/2611.21258)、[作者项目页](https://thinkwam-project.github.io/)。
