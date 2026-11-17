# 🧑‍💻 Foundation Model Role Map | 基座模型人才岗位地图

> A technical role framework for talent conversations, **not a verified list of current job openings**.  
> 用技术工作内容理解人才画像；**这不是实时招聘岗位表**。

[← Back to Radar](../README.md)

## 1. Why a role map? | 为什么要做岗位地图？

团队对岗位的命名并不统一。“大模型算法”可能意味着模型架构、预训练数据、分布式训练、后训练或应用研发。判断人才匹配度，应优先理解**本人实际解决的问题、所处训练阶段、产出与技术深度**，而不是仅依靠岗位名称。

## 2. Core role families | 核心岗位分类

| Role family | Technical ownership / 主要负责内容 | Signals to verify / 核验要点 |
| --- | --- | --- |
| **LLM pre-training research** | 模型架构、预训练目标、scaling 和训练实验 | 是否亲自设计训练实验、如何解读训练曲线及评测 |
| **Pre-training data** | 训练语料、数据质量、去重与配比 | 数据实验设计、质量指标、数据治理能力 |
| **Multimodal foundation research** | 图文、视频、音频等跨模态基础建模 | 基础预训练还是在现有模型上微调 |
| **Image/video generative research** | 扩散 / 流模型、生成架构、时空建模 | 视频基座训练与后期编辑、超分是否区分 |
| **Distributed training systems** | 并行、通信、训练吞吐、容错与稳定性 | 实际负责的训练系统问题和技术改进 |
| **Model evaluation** | 训练中能力评估、基准设计、污染检查 | 是否能解释指标变化与评测局限 |
| **Post-training / RL** | SFT、偏好优化、RL 训练等 | **相邻但不同于基座预训练**，不能混称 |
| **Agent applications** | Tool use、任务编排、系统集成、应用评测 | 侧重应用工程还是训练模型的 Agent 能力 |
| **Inference / serving** | 模型部署、推理吞吐、延迟和成本 | 不应与训练系统岗位自动等同 |

## 3. Five-dimensional candidate profile | 五维人才画像

评估一个人的工作时，可以整理以下五个维度：

1. **Model stage / 阶段**：Pre-training、post-training、inference、application。
2. **Modality / 模态**：Text、vision-language、image、video、audio。
3. **Primary ownership / 主责**：算法、数据、训练系统、评估、产品工程。
4. **Evidence / 证据**：公开论文、代码、技术报告、可合规分享的项目成果。
5. **Career direction / 职业意向**：研究型、工程型、研究工程混合型、技术管理。

**不应索取**保密模型参数、客户资料、候选人私密记录，或任何未获授权的内部业务信息。

## 4. Example: similar titles, different work | 相似职位的不同含义

**“Multimodal Engineer”** 可能是：
- 研究视觉语言基础表征和大规模联合预训练；
- 进行已有视觉语言模型的指令微调和后训练；
- 构建 OCR / 视频理解 / Agent 等应用工作流。

这三种经历可能都有价值，但目标岗位与技能验证方法并不相同。

**“AI Infra Engineer”** 可能是：
- 训练集群和分布式通信；
- 数据平台与训练流水线；
- 推理 serving / 部署优化。

具体匹配仍取决于团队的实际工作内容。

## 5. How to use this map | 使用方式

- 与研究员交流时，用**技术问题和实际贡献**核验方向，避免拿 buzzwords 机械匹配。
- 对公开 JD 做拆解时，标明**招聘原文**与**分析推断**。
- 做行业内容时，**不要把技术趋势误写成某家公司确定正在扩招**。
- 对任何简历或职业背景信息，先取得使用许可，并避免公开可识别个人的敏感信息。

## 6. Planned extensions

- 预训练研究员与训练系统工程师的能力边界
- 多模态视频生成基座人才画像
- 研究员 / Research Engineer / Infra Engineer 的角色区分
- 技术负责人和研发一号位的能力维度

[Source policy](../methodology/source-policy.md) · Updated: 2026-11-17
