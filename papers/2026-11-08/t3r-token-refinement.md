# T3R: Training-Free Two-Stage Token Refinement Towards Efficient and Robust VLA Models

- **作者**：Mohammed Hassan、Zhenyang Chen、Zheng Wang、Zhixin Zhu、Tianlong Chen、Yingyan (Celine) Lin、Chaojian Li
- **首次公开**：2026-11-05；**状态**：arXiv 预印本
- **论文**：[arXiv](https://arxiv.org/abs/2611.08413)；**项目页/代码**：官方摘要未提供可核实链接。

## 研究问题
多相机 VLA 每步处理大量视觉 token，既增加推理成本，也可能被与动作无关的背景干扰。

## 核心方法
无需重新训练：先用分割引导删除不相关视觉块，再以显著性引导的注意力偏置，把保留 token 的注意力分配给动作关键区域与指令。

## 实验任务与主要结果
在 LIBERO、SIMPLER、RoboTwin 的三种 VLA 骨干上评估。LIBERO-Spatial 可删去场景相机 85% 的视觉 token，基本保持原成功率；分布外物体位置扰动下最高提升 7 个百分点。作者报告高分辨率时 LLM 前向计算最高加速 3.3 倍，但剪枝与注意力偏置每次调用需要 7.8 毫秒。

## 对 VLA 的价值
提供可移植的推理阶段准确率与计算量折中方法，尤其适合多相机机器人策略。

## 局限或待验证点
3.3 倍是 LLM 前向部分的性能，并非端到端机器人控制速度；收益依赖分割质量，真实机器人长程任务需验证。

**核验来源**：[arXiv 官方摘要](https://arxiv.org/abs/2611.08413)。
