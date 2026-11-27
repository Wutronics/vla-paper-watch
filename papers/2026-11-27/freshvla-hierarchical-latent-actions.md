# FreshVLA: Frequency-Regularized Time Scale Hierarchical Latent Actions for Vision-Language-Action Models

- **作者**：Jiaming Liang、Yifeng Zhan、Rongyi He、Mu Li、Jiaqi Fan、Zhiyuan Zhang、Qiwei Liang、Zhengjie Zhang、Boyang Cai、Ningyuan Zhang、Xingjian Jing、Qiang Nie
- **机构**：香港科技大学（广州）、小鹏机器人、同济大学上海智能科学技术研究院、香港城市大学（作者项目页）
- **首次公开**：2026-11-25；**状态**：arXiv 预印本，未核实正式录用
- **论文**：[arXiv](https://arxiv.org/abs/2611.33635)；**项目页**：[FreshVLA](https://freshvla.github.io/)；**代码**：[GitHub 占位仓库，代码待发布](https://github.com/FreshVLA/FreshVLA)。

## 研究问题
从无动作标注视频学习的潜在动作容易编码静态场景外观，并把缓慢任务进展和快速执行细节混在一起，因而未必能改善机器人策略。

## 核心方法
先用时间高通视觉先验聚焦变化区域，再以跨时间尺度采样和频域约束学习连续的双层潜在动作：较慢分支表示任务阶段，较快分支表示局部执行残差。训练 VLA 时冻结视频编码器，以联合流匹配同时生成潜在动作和机器人动作；推理时仅执行机器人动作。相对重建导向的单层或离散潜在动作，核心改动是显式分离动态时间尺度。

## 实验与主要结果
在 227,894 条真实及仿真轨迹上预训练。LIBERO 四套任务平均成功率 98.2%，其中 LIBERO-Long 98.0%，高于 GR00T-N1.6 的 94.4%；CALVIN 平均连续完成 4.52/5 项子任务；零样本 LIBERO-PLUS 平均 80.4%。四项 Flexiv 真机桌面任务平均成功率 84.2%，高于 π₀.₅ 的 76.7%（每任务收集 30 条轨迹）。去掉潜在动作时 LIBERO 平均降至 96.0%、Long 降至 93.0%；去掉频域约束时 Long 同样降至 93.0%。论文还比较多种潜在动作结构与时间粒度。

## 研究价值
展示如何把无动作视频中的时间结构转成 VLA 的训练监督，并在长程任务、视觉扰动与真机操作中验证增益。双时间尺度的连续潜在动作值得在其他模型与视频语料上复现。

## 局限与待验证点
真实机器人仅一类机械臂和四项桌面任务，跨形态泛化仍待验证。LIBERO-Goal 为 96.3%，低于部分强基线；作者认为潜在动作预训练缺少显式语言目标条件。项目链接的仓库目前只有待发布说明，代码尚不可复现。

## 综合质量评价
- **AI 综合评分**：86/100（创新 22/25；实验 23/25；研究价值 19/20；真机与泛化 17/20；可复现性 5/10）。
- **依据与推荐**：强基线、跨基准评估、真机和分量消融支撑核心结论；尚未公开代码且真机范围有限。**阅读优先级：推荐**。

**核验来源**：[arXiv 官方摘要](https://arxiv.org/abs/2611.33635)、[论文 HTML 原文](https://arxiv.org/html/2611.33635)、[作者项目页](https://freshvla.github.io/)。评分为 AI 辅助研究判断，并非官方评级。
