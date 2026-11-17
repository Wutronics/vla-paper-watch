# ScaleVLA: Scaling Vision-Language-Action Models to 552 Billion Parameters

- **作者**：Ruixi Yu、Dairu Liu、Xuchuan Chen、Zekun Qi、Zekai Li、Zhuo Cao、Luyang Niu、Yingsheng Zhang、Sikai Liang、Ke Fan、He Wang、Li Yi
- **首次公开**：2026-11-16；**状态**：arXiv 技术报告
- **论文**：[arXiv](https://arxiv.org/abs/2611.21607)；**项目页/代码**：官方摘要未提供可核实链接。

## 研究问题
现有 VLA 通常使用远小于前沿视觉语言模型的骨干；研究考察更大规模表征能否改善示范效率、泛化和精细操作。

## 核心方法
把 552B DeepSeek-V4.1-Flash 视觉语言骨干连接到可训练的动作 DiT，在统一训练设置下与 2B 至 552B 不同规模骨干比较。

## 实验任务与主要结果
作者报告，10 条示范的 552B 模型成功率 87.8%，高于 50 条示范的 2B 模型 85.6%；LIBERO-PRO 成功率 45.1%，较小骨干最高 31.3%。真实充电器插入由 4/10 提升到 9/10 次成功；每个动作块中位延迟 216 毫秒。

## 对 VLA 的价值
为大规模视觉语言骨干作为动作策略表征基础的收益与时延权衡提供直接比较。

## 局限或待验证点
552B 部署成本高；真实机器人实验规模较小，延迟数字也需结合硬件、动作频率与端到端控制要求理解。

**核验来源**：[arXiv 官方摘要](https://arxiv.org/abs/2611.21607)。
