# LoopQ: Fair, Closed-Loop Evaluation of Quantized Vision-Language-Action Models

## 基本信息

- **作者**：Syed Umer Bukhari、Magnus Almgren、Ahmed Ali-Eldin
- **首次公开**：2026-11-03
- **会议/状态**：arXiv 预印本（arXiv:2611.05093）
- **论文**：[arXiv 摘要页](https://arxiv.org/abs/2611.05093)
- **项目页/代码**：未发现作者提供的可核实链接。

## 研究问题
VLA 后训练量化研究常用不同检查点、量化层或推理引擎比较，难以判断专用算法是否真的胜过简单基线，也难判断内存收益能否转成控制延迟收益。

## 核心方法
LoopQ 固定检查点、量化范围与运行环境，只改变量化方法和内核；比较 RTN、AWQ、GPTQ 与 VLA 专用方法，在 LIBERO、LIBERO-plus 上闭环评估四种 VLA，并测量 H100、L4 和 Jetson AGX Thor 的内存与时延。

## 实验任务与主要结果
超过 18 万次闭环操作评估显示，低位量化能节省约 2–3 倍模型内存，但多种 VLA 专用方法不优于通用 RTN/AWQ/GPTQ。标准 LIBERO 看不出的性能损失在 LIBERO-plus 配对扰动下可达 1.5–4.3 个百分点。H100 上受测 π0.5 和 OpenVLA-OFT 量化配置没有快于对应 16 位模型，部分配置反而慢 1.06–1.58 倍。

## 对 VLA 的价值
为机器人策略部署提供更可信的量化比较协议：同时看闭环成功率、分布扰动、真实低位内核和端到端时延，避免仅凭位宽或静态指标推断控制收益。

## 局限或待验证点
部分模型只做模拟量化，不能支持真实速度结论；速度结果限于三个 GPU 与批量为 1 的场景，更大批量或新内核可能改变排名。

## 核验来源

- [arXiv 官方摘要页](https://arxiv.org/abs/2611.05093)
