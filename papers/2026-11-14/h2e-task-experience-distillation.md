# What Can a VLA Learn from the Agent That Calls It? Task-Level Experience Distillation for Embodied Navigation

- **作者**：Jinze Tao、Yuxiao Han、Kangkang Dong、Yancong Wei、Xiaojun Zhu、Bokui Chen、Houde Liu
- **首次公开**：2026-11-12；**状态**：arXiv 预印本
- **论文**：[arXiv](https://arxiv.org/abs/2611.16246)；**项目页/代码**：官方摘要未提供可核实链接。

## 研究问题
导航系统常由语言模型规划器反复调用 VLA，带来每轮成本和时延；规划器的成功交互轨迹又不能直接视作标准 VLA 示范。

## 核心方法
H2E 把代理会话中的动作映射到原始任务指令，使用到达姿态作为监督目标，屏蔽远离目标的步骤，并把目标一米内的状态标为停止，再以低秩适配更新 VLA。

## 实验任务与主要结果
在 REVERIE-CE 的全部 3,189 个未见验证情节上，8B VLA 的导航成功率由 35.0% 升至 44.9%，测试时无需语言模型规划器。

## 对 VLA 的价值
说明可以把高层代理成功经验蒸馏进直接控制的 VLA，减少部署时持续调用规划模型。

## 局限或待验证点
当前证据集中于具身导航；将此任务级经验转化用于接触丰富的机器人操作，仍需独立验证。

**核验来源**：[arXiv 官方摘要](https://arxiv.org/abs/2611.16246)。
