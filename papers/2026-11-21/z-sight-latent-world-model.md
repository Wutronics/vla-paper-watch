# $Z$-sight: Unifying Vision-Language-Action and Latent World Modeling

- **作者**：Junjie Ye、Yiqi Zhao、Muchen Xu、Celina Shiyu Wang、Hao Dong、Ruohai Ge、Rong Xue、Benjamin J Kolligs、Aditya Dutt、Sasanka Nagavalli、Nassim A. Samad、Gaurav S. Sukhatme、Jyotirmoy V. Deshmukh、Yue Wang、Yuliang Guo
- **首次公开**：2026-11-18；**会议/状态**：arXiv 预印本，未见官方会议录用信息
- **论文**：[arXiv](https://arxiv.org/abs/2611.24940)；**项目页**：[$Z$-sight](https://junjieye.com/Z-sight/)；**代码**：项目页所列代码链接核验时不可访问，暂不收录。

## 研究问题
视频生成式世界动作模型能预测未来，却带来较高生成开销；只预测紧凑潜在特征的方法又可能与持续适应的视觉骨干脱节。论文探索如何在 VLA 自身表征空间里预测未来并用于控制。

## 核心方法
模型在视觉语言骨干旁设置未来视觉 token 专家和连续动作专家，并在混合 Transformer 中联合去噪。未来目标由视觉编码器的指数滑动平均教师提供；预测未来无需重建图像，也无需外部冻结编码器。训练结合人类视频与机器人轨迹。

## 实验任务与主要结果
作者报告，SIMPLE 人形机器人基准的平均成功率为 81.9%，比最强对照高 9.6 个百分点；Unitree G1 六项真实任务平均为 73.3%，高 20.0 个百分点。每个动作块约需 110 毫秒，并在桌面操作基准保持竞争力。

## 对 VLA 的价值
展示了用策略自身的视觉 token 表征构建轻量未来预测，再将其直接用于动作生成的路径，为世界模型与 VLA 融合提供实证。

## 局限或待验证点
真实机器人结果来自六项 G1 任务，跨机器人与更复杂开放环境的泛化仍需验证；吞吐与时延取决于硬件和动作块设置。

**核验来源**：[arXiv 官方摘要](https://arxiv.org/abs/2611.24940)、[作者项目页](https://junjieye.com/Z-sight/)。
