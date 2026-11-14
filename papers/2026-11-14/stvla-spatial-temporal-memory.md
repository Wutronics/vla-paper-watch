# STVLA: Spatial-aware and Temporal-memory forVision-Language-Action Models

- **作者**：Zhuo Han、Yeqiang Wang、Xinran Wang、Hongwei Han、Yi Xiong、Zunian Wan、Jianbo Mao、Huan Peng、Yongcheng Liu、Wei Shan、Maoqing Yao
- **首次公开**：2026-11-12；**状态**：arXiv 预印本
- **论文**：[arXiv](https://arxiv.org/abs/2611.16589)；**项目页**：[STVLA](https://stvla.github.io/)；**代码**：未发现可核实仓库。

## 研究问题
仅看当前图像的 VLA 难以区分相似画面下的不同任务阶段；只记视觉外观又容易受到遮挡和视角变化影响。

## 核心方法
把预训练视觉几何模型的空间特征和视觉特征一同放入有界时序记忆，并按与当前观测的相关性及信息互补性选择历史，再用于动作生成。

## 实验任务与主要结果
在 LIBERO、LIBERO-Mem、MIKASA-Robo 和 SimplerEnv Bridge 上，作者报告平均成功率均高于所比较方法。AGIBOT G2 真实机器人三项任务的平均成功率为 76.7%，其中积木堆叠 100%、物体整理 85%、手机包装 45%；相较 π0.5 分别提高 58.33、30.00、35.00 个百分点。

## 对 VLA 的价值
为需要空间精度和任务历史的长程操作提供视觉与几何联合记忆设计，并展示真实机器人结果。

## 局限或待验证点
真实实验只有三类任务；手机包装成功率仍为 45%，几何编码和记忆检索的计算成本也需评估。

**核验来源**：[arXiv 官方摘要](https://arxiv.org/abs/2611.16589)、[作者项目页及结果表](https://stvla.github.io/)。
