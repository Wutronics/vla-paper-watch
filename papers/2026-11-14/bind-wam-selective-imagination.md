# Bind-WAM: Binding-Uncertainty-Guided Selective Future Imagination in World Action Models

- **作者**：Chenhao Qiu、Shuyi Chen、Songen Gu、Shufeng Nan、Tianyu Wang、Siyu Lin、Yifan Li、Bingwen Zhu、Yanwei Fu
- **首次公开**：2026-11-11；**状态**：arXiv 预印本
- **论文**：[arXiv](https://arxiv.org/abs/2611.15368)；**项目页/代码**：官方摘要未提供可核实链接。

## 研究问题
世界动作模型每次重规划都生成未来视觉状态成本较高，且有些时候无需想象；关键是判断何时未来预测真正有助于执行。

## 核心方法
用语言与物体的绑定不确定性判断当前观测能否稳定支持动作。离线从完整示范标记指代不匹配、目标不可见与身份漂移，训练轻量路由器；推理时根据不确定性及变化选择是否调用未来图像与动作联合生成。

## 实验任务与主要结果
作者报告在仿真和真实机器人实验中，选择性未来想象有助于控制且可解释；官方摘要未给出具体成功率或延迟数值，量化收益需查看正文实验表。

## 对 VLA 的价值
提供按语义指代风险分配推理计算的机制，可借鉴于需要未来预测的 VLA 与世界动作模型。

## 局限或待验证点
伪标签依赖完整示范和动作上下文；路由错误可能在目标遮挡或指令歧义下漏掉关键重规划，且摘要缺少端到端速度数据。

**核验来源**：[arXiv 官方摘要](https://arxiv.org/abs/2611.15368)。
