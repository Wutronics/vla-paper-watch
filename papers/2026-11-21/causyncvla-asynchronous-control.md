# CauSyncVLA: Causal Latent World Modeling for Asynchronous Robot Control

- **作者**：Xu Pan、Chubin Zhang、Xingrui Yu、Runmin Lan、Zihao Wang、Wenkai Guo、Bofang Jia、Bo An、Ziwei Wang
- **首次公开**：2026-11-19；**会议/状态**：arXiv 预印本，未见官方会议录用信息
- **论文**：[arXiv](https://arxiv.org/abs/2611.25667)；**项目页/代码**：官方摘要未提供可核实链接。

## 研究问题
异步 VLA 可让推理和机器人执行重叠，但视觉推理完成时感知记忆可能已经过时，连续动作块之间也可能出现不连贯。

## 核心方法
双系统控制器利用延迟视觉锚点与已执行的状态、动作历史，预测当前的潜在感知记忆；再用预测式流模型热启动，对尚未执行的动作轨迹做单步校正。感知记忆通过对动作敏感的蒸馏训练，而动作校正无需额外训练。

## 实验任务与主要结果
作者报告在 LIBERO-10 上取得 93.8% 成功率，同时达到 5.04 倍推理吞吐，并改善闭环鲁棒性与机器人运动平滑性。

## 对 VLA 的价值
针对 VLA 实际部署中的计算延迟与动作连续性，提供将潜在世界模型用于异步控制的方案。

## 局限或待验证点
官方摘要主要报告 LIBERO-10 结果；真实机器人上不同网络延迟、控制频率与干扰条件下的收益仍需验证。

**核验来源**：[arXiv 官方摘要](https://arxiv.org/abs/2611.25667)。
