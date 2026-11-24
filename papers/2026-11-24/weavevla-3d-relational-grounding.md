# WeaveVLA: 3D Relational Grounding for Vision-Language-Action Models

- **作者**：Zien Wang、Yuhao Pan、Yunfeng Fan、Nan Cheng、Xin Xia、Wenchao Xu
- **机构**：香港科技大学、香港理工大学、西安电子科技大学、浙江大学（论文 HTML 正文）
- **首次公开**：2026-11-23；**状态**：arXiv 预印本，未核实正式录用
- **论文**：[arXiv](https://arxiv.org/abs/2611.31126)；**项目页**：[WeaveVLA](https://kingzein.github.io/weave-vla/)；**代码**：[GitHub](https://github.com/Kingzein/WeaveVLA)。

## 研究问题
VLA 对与任务有关的物体、夹爪及参考点之间的三维关系往往只作隐式编码，视角和初始状态改变时易失效。

## 核心方法
根据指令构建稀疏三维关系图，针对每对实体维护跨观测更新的循环边状态；图神经网络和查询读出将关系压缩为 token，与原视觉语言上下文共同条件化动作专家。区别于全连接场景图，关系选择和历史更新均受任务约束。

## 实验与主要结果
在 StarVLA-GR00T 和 π₀.₅ 两种骨干上评估。LIBERO-Plus 分别由 74.9% 升至 82.0%、85.7% 升至 87.8%；三项真实任务中，StarVLA-GR00T 版本在常规条件由 55.6% 升至 70.0%，分布外扰动由 33.3% 升至 53.3%。另有 CALVIN 与关系模块消融；π₀.₅ 的 LIBERO-Plus 增益相对较小。

## 研究价值
明确表示并维护操作过程中的三维关系，为 VLA 空间泛化提供可插入不同动作骨干的模块。

## 局限与待验证点
依赖检测、跟踪及三维估计质量；真实任务仅三项，复杂遮挡下稳定性仍待验证。

## 综合质量评价
- **AI 综合评分**：84/100（创新 20/25；实验 22/25；研究价值 18/20；真机与泛化 17/20；可复现性 7/10）。
- **依据与推荐**：跨两种骨干、仿真与真机扰动及消融支持其价值；代码与部分模型权重已公开，但前端几何依赖仍高。**阅读优先级：推荐**。

**核验来源**：[arXiv 官方摘要](https://arxiv.org/abs/2611.31126)、[arXiv 正文](https://arxiv.org/html/2611.31126v1)、[作者项目页](https://kingzein.github.io/weave-vla/)、[代码仓库](https://github.com/Kingzein/WeaveVLA)。评分为 AI 辅助判断，并非官方评级。
