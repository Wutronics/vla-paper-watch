# PhyDEX: A Benchmark for Physical Reasoning in Vision-Language-Action Models via Dynamic Extrinsic Dexterity

- **作者**：Hao Vo、Taisei Hanyu、Yuki Ikebe、Pham Tri Quang、Sreevenkata Anjani Tishita Godavarthi、Nghi D. Q. Bui、Daniel Sonntag、Chase Rainwater、Duy Minh Ho Nguyen、Anh Nguyen、Ngan Le
- **首次公开**：2026-11-19；**会议/状态**：arXiv 预印本，未见官方会议录用信息
- **论文**：[arXiv](https://arxiv.org/abs/2611.26565)；**项目页/代码**：官方摘要未提供可核实链接。

## 研究问题
现有机器人操作基准侧重夹爪与物体接触，难以测出 VLA 是否能理解质量、重心、摩擦和惯性对动作结果的影响。

## 核心方法
PhyDEX 将动态外在灵巧操作具体化为投掷任务：机器人要估计物体物理属性，将物体送到机械臂工作空间之外的目标。自动化数据生成流程结合抓取生成、运动规划、闭环投掷优化与物理参数随机化，形成九类任务、100 个场景和约 3.5 万条轨迹。

## 实验任务与主要结果
数据共约 143 小时，覆盖形状不规则、质量动态变化的物体，以及静态、多个和移动目标。作者测试 GR00T N1.7、DynamicVLA 与 ForceVLA，三者成功率均低于 3%；提供真实物理属性后，成功率约翻倍。人形机器人和真实世界实验也出现相似失效模式。

## 对 VLA 的价值
提供了面向物理推理的诊断基准，可区分抓取前的基本鲁棒性问题与对物体动力学的感知不足。

## 局限或待验证点
总体成功率极低，部分失败发生在投掷之前，因此不能把全部失败归因于物理推理；任务集中于投掷，尚不能代表所有接触操作。

**核验来源**：[arXiv 官方摘要](https://arxiv.org/abs/2611.26565)。
