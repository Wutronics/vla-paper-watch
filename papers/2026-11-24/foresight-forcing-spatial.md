# Foresight Forcing: Learning Spatial Foresight for Robotic Manipulation

- **作者**：Mishuo Han、Zhixuan Liang、Zhaoyuan Wan、Wendi Chen、Jiarui Chen、Xinkai Wang、Yue Ma、Yu Zhou、Junting Chen、Yao Mu、Jun Lv、Chuan Wen、Cewu Lu
- **机构**：上海交通大学、香港大学、上海创智学院、Noematrix、复旦大学、香港科技大学、新加坡国立大学（作者项目页）
- **首次公开**：2026-11-23；**状态**：arXiv 预印本，未核实正式录用
- **论文**：[arXiv](https://arxiv.org/abs/2611.30963)；**项目页**：[Foresight Forcing](https://anson2333.github.io/foresight-forcing/)；**代码**：[GitHub](https://github.com/anson2333/ForesightForcing)。

## 研究问题
视频式世界动作模型预测未来画面时，物体关系变化和三维几何转移仍隐含在像素里，监督信号容易混入外观与视角变化。

## 核心方法
冻结三维基础模型提取当前与未来对齐图像的分块特征差，作为空间转移目标；策略从当前观测、语言及本体状态预测转移查询，并把查询提供给动作专家。部署不需要未来图像或三维教师，区别于直接生成未来 RGB 的方法。

## 实验与主要结果
在 LIBERO、LIBERO-Plus 和 RoboTwin 2.0 上测试，RoboTwin 2.0 Full 平均成功率 95.01%。六项真实双臂长程操作的平均任务得分 85.8%，项目页给出的 π₀.₅ 与 ImageWAM 分别为 83.5% 和 70.2%。论文有空间监督与动作条件的消融；相对强 VLA 基线的真机增量较小。

## 研究价值
把三维关系变化蒸馏为动作生成所用的未来表征，为无需部署重型未来图像生成器的 VLA 提供可复用思路。

## 局限与待验证点
训练依赖冻结三维模型和跨时刻对齐；真实任务得分对 π₀.₅ 的优势仅 2.3 个百分点，需在更多平台检验稳定性。

## 综合质量评价
- **AI 综合评分**：84/100（创新 21/25；实验 21/25；研究价值 18/20；真机与泛化 16/20；可复现性 8/10）。
- **依据与推荐**：有跨基准和六项真机任务，项目和代码公开；强基线真机优势有限。**阅读优先级：推荐**。

**核验来源**：[arXiv 官方摘要](https://arxiv.org/abs/2611.30963)、[作者项目页](https://anson2333.github.io/foresight-forcing/)、[代码仓库](https://github.com/anson2333/ForesightForcing)。评分为 AI 辅助判断，并非官方评级。
