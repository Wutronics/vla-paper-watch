# ManiLadder: Benchmarking Robot Manipulation Through a Categorized and Multi-Difficulty Level Task Ladder

- **作者**：Chongkai Gao、Jieao Shi、Zhaoyu Mu、Yudi Lin、Xuanwei Liu、Wei Ken Ng、Baiye Cheng、Anqi Chen、Kerun Liu、Zhuoran Li、Xuchuan Huang、Haoyang Li、Shengjia Zhu、Nga Teng Chan、Yuxuan Zhang、Xingyu Chen、Lin Shao
- **首次公开**：2026-11-12；**状态**：arXiv 预印本
- **论文**：[arXiv](https://arxiv.org/abs/2611.16374)；**项目页/代码**：arXiv 所列项目地址目前不可访问，未核实到代码。

## 研究问题
现有操作基准常集中在简单抓取放置，缺少按难度系统分层的任务集，难以衡量策略跨技能和难度的进步。

## 核心方法
构建 112 项仿真任务，按 4 个难度等级和每级 8 类组织，覆盖刚体、可变形物、单/双臂与灵巧手。在统一数据量和流匹配模仿学习协议下，以成功率校准经验难度，并跨随机种子和策略验证。

## 实验任务与主要结果
作者比较不同策略、数据规模和任务迁移，并以真实机器人实验检查任务难度顺序能否延续到物理世界。摘要未给出统一排行榜数值，因此不在此写具体成功率。

## 对 VLA 的价值
为 VLA 操作策略提供分层评估：可分开考察任务类别、难度、数据扩展和真实世界迁移。

## 局限或待验证点
难度以特定统一策略的成功率操作化，可能随模型能力变化；仿真与真实机器人之间的一致性仍需更多平台验证。

**核验来源**：[arXiv 官方摘要](https://arxiv.org/abs/2611.16374)。
