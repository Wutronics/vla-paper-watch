# Failure Prediction and Classification in Vision-Language-Action Models Via Calibrated Latent Probing

- **作者**：Michal P. Podolinsky、Yunhao Yang、Daniel Little、Hong Lu、Rohan Siva、Olin Goudey、Neel P. Bhatt、Matthias Scheutz、Ufuk Topcu
- **首次公开**：2026-11-05；**状态**：arXiv 预印本，作者项目页称投稿审稿中
- **论文**：[arXiv](https://arxiv.org/abs/2611.08425)；**项目页**：[VLA-Tug](https://vla-tug.github.io/)；**代码**：[匿名审稿镜像](https://anonymous.4open.science/r/VLA-Tug/)。

## 研究问题
VLA 在分布变化下可能突然失败；部署时需要能提前报警、控制误报漏报，并指出失败类型的低开销监测器。

## 核心方法
在 VLA 骨干潜在特征上训练轻量时序探针，利用失败前轨迹监督故障分数和类型；在留出轨迹上校准报警阈值，并把预测结果用于停止或转交控制。

## 实验任务与主要结果
在 LIBERO-10、LIBERO-X 和真实机器人轨迹上评估；论文摘要报告，相同误报率下早期故障检测比最强学习基线最高提升 30%，未见任务中错误率界限在最高 86% 的运行中有效（基线最多 21%），失败类型 top-3 准确率最高提升 44%。作者报告 3,180 条标注操作轨迹。

## 对 VLA 的价值
为 VLA 闭环部署提供可校准的故障预警与失败类型线索，可与原策略并行工作。

## 局限或待验证点
项目页仍有待更新占位内容，数据集链接标注为即将提供；误报和漏报保证依赖校准数据及其适用假设，长期部署需继续检验。

**核验来源**：[arXiv 官方摘要](https://arxiv.org/abs/2611.08425)、[作者项目页](https://vla-tug.github.io/)。
