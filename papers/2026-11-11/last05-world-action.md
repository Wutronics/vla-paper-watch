# LaST0.5: A Generalist World Action Model with Interaction-Centric Latent Reasoning

- **作者**：Xuheng Zhang、Yiming Zhang、Jialin Gao、Hao Chen、Jiaming Liu、Ji Li、Runzhong Huang、Yinxi Wang、Chenyang Gu、Zihan Yang、Yaowei Liu、Zhonghao Yan、Ziyu Guo、Renrui Zhang、Peng Jia、Pheng-Ann Heng、Shanghang Zhang
- **首次公开**：2026-11-10；**状态**：arXiv 预印本
- **论文**：[arXiv](https://arxiv.org/abs/2611.14048)；**项目页/代码**：官方摘要未提供可核实链接。

## 研究问题
世界动作模型的全局场景表征可能忽略机器人与物体的局部接触，使视频预测知识难以有效转化为操作动作。

## 核心方法
在世界专家与动作专家之间加入交互潜在专家，利用机器人和环境的视觉交互线索学习紧凑表征；同时预测未来表征和任务进度，并按进度一致性调整执行和重采样。模型以逾 1.4 万小时机器人数据预训练。

## 实验任务与主要结果
作者报告 LIBERO 成功率 99.5%，在十项 RLBench 任务上超过先前最优结果，并展示真实机器人长程执行与精细灵巧操作；摘要未给出后两类实验的完整量化数值。

## 对 VLA 的价值
将可解释的局部交互建模置于世界模型与动作策略之间，为长程 VLA 和 WAM 的物理推理提供架构参考。

## 局限或待验证点
大规模预训练的成本较高；公开摘要缺少真实实验详细成功率，外部复现与推理延迟仍待核查。

**核验来源**：[arXiv 官方摘要](https://arxiv.org/abs/2611.14048)。
