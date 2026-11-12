# VLA-MOPD: On-Policy Distillation for Multi-Task VLA Policy Consolidation

- **作者**：Yongxuan Lv、Zhen Fang、Lichen Man、Hao Li、Pu Li、Hengyi Wang、Langfeng Cao、Lin Chen、Jie Huang、Xiu Su、Shan You、Fei Wang、Feng Zhao
- **首次公开**：2026-11-09；**状态**：arXiv 预印本
- **论文**：[arXiv](https://arxiv.org/abs/2611.12286)；**项目页/代码**：官方摘要未提供可核实链接。

## 研究问题
为不同任务微调出的 VLA 专家难以合并成一个策略；离线蒸馏忽略学生实际访问的状态，只监督最终动作也遗漏流匹配生成过程。

## 核心方法
共享学生策略在线采集轨迹，在访问的观察与中间 ODE 状态查询按指令路由的冻结教师，以局部流步转移目标训练有效动作块；可选参考策略项减少旧任务遗忘。

## 实验任务与主要结果
从每个 LIBERO 任务一条轨迹出发，平均单次成功率由 75.4% 升至 98.9%；RoboTwin 2.0 由 73.0% 升至 89.3%；Piper 真实机器人两轮合并后平均成功率由 70.0% 升至 90.0%。

## 对 VLA 的价值
提供多任务流匹配 VLA 的在线专家合并方法，兼顾学生实际状态分布与已学技能保留。

## 局限或待验证点
训练需要多位冻结教师及在线机器人轨迹，计算和采样成本可能较高；跨具身合并仍待验证。

**核验来源**：[arXiv 官方摘要](https://arxiv.org/abs/2611.12286)。
