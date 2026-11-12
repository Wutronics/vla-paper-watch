# DexSeed: Expanding Human Hand-Object Interactions into Robot Demonstrations for Dexterous Policy Learning

- **作者**：Huaijin Pi、Zehong Shen、Yong Wang、Kechun Xu、Changpeng Wang、Dingkun Wei、Xueyang Wang、Wenjia Wang、Xing Zhu、Yujun Shen、Taku Komura
- **首次公开**：2026-11-10；**状态**：arXiv 预印本
- **论文**：[arXiv](https://arxiv.org/abs/2611.14092)；**项目页**：[DexSeed](https://robbyant-research.github.io/DexSeed/)；**代码**：[GitHub](https://github.com/robbyant-research/DexSeed)。

## 研究问题
灵巧 VLA 需要覆盖不同物体、抓取方式与位置的可执行示范，而遥操作采集昂贵，直接重放人手交互又缺少变化。

## 核心方法
按抓取模式组织人手与物体交互，进行机器人手重定向、物体几何和手臂轨迹扩展；以强化学习手指策略和物理仿真筛选可执行轨迹，再将渲染观察、动作与语言描述配对训练 VLA。

## 实验任务与主要结果
作者项目页列出 19 条人类源序列、8 种抓取模式、17 类物体及 25,270 条生成机器人轨迹。匹配手臂参考的仿真执行实验中，方法成功率 95.50%，比较方法为 24.81%–34.25%；仅用生成示范微调的 VLA 还在真实机器人上完成语言指定抓取。

## 对 VLA 的价值
把少量人手交互扩展为有语言条件、物理可执行的灵巧操作数据，为低成本 VLA 数据扩容提供路线。

## 局限或待验证点
生成轨迹依赖仿真、重定向与手指控制质量；项目页真实机器人展示未给出统一的总体成功率，跨物体和跨手型泛化需继续验证。

**核验来源**：[arXiv 官方摘要](https://arxiv.org/abs/2611.14092)、[作者项目页](https://robbyant-research.github.io/DexSeed/)。
