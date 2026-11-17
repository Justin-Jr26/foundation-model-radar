# 🎬 Generative Models | 生成模型与基座训练

> A foundation-model view of image and video generation.  
> 核心关注**图像 / 视频生成基座模型**，而非仅关注推理调用或创作工具。

[← Back to Radar](../README.md)

## 1. Scope | 研究范围

生成模型旨在学习数据分布，并据此生成内容。图像和视频生成中，需要区分：

- **基础生成建模**：训练目标、网络结构、扩散 / 流模型路线等。
- **条件生成**：如何接入文本、图像或其他条件信号。
- **视频时空建模**：运动、时序一致性、长序列与镜头变化。
- **数据与训练工程**：数据筛选、视频解码、分辨率与帧数、吞吐和稳定性。
- **后续阶段**：偏好优化、推理加速、超分、编辑和应用工具等，不必然属于基座训练。

*注：本项目不会把“生成效果好”直接推导为“基座模型强”。结论依赖评价维度与实验条件。*

## 2. Major research questions | 技术观察框架

| 方向 | 需要理解的问题 | 常见人才标签 |
| --- | --- | --- |
| **Diffusion** | 正向加噪与去噪生成的训练思路是什么？ | Generative modeling, diffusion |
| **Latent-space modeling** | 在压缩潜空间建模可以带来什么计算取舍？ | Autoencoding, latent modeling |
| **Transformer backbone** | 生成模型为何采用 Transformer 结构、如何扩展？ | DiT, architecture, scaling |
| **Video generation** | 时间一致性、运动动态、长视频训练如何处理？ | Video foundation models, temporal modeling |
| **Systems & data** | 训练吞吐、高质量视频数据与评估如何影响路线？ | Training systems, video data |

## 3. Foundational reading | 经典文献

- **Denoising Diffusion Probabilistic Models** (2020) — 扩散概率模型的经典训练研究。[Paper](https://arxiv.org/abs/2006.11239)
- **High-Resolution Image Synthesis with Latent Diffusion Models** (2021/2022) — 在潜空间执行生成建模，以平衡质量和计算成本。[Paper](https://arxiv.org/abs/2112.10752)
- **Scalable Diffusion Models with Transformers** (2022) — 研究 Transformer 主干在扩散模型中的可扩展性。[Paper](https://arxiv.org/abs/2212.09748)

这些是技术脉络的起点，**不是**对当下所有最新视频基座路线的完整覆盖。

## 4. Role map | 人才观察

- **生成模型基座研究员**：目标函数、架构、训练策略、尺度与评测。
- **视频生成研究员**：时空表示、运动一致性、长视频建模。
- **生成模型数据研究 / 工程**：图像 / 视频清洗、标注、过滤、字幕与数据管线。
- **分布式训练 / 性能工程师**：高分辨率数据与训练体系下的吞吐、稳定性与集群效率。
- **后训练 / 推理优化工程师**：重要但与从零基座训练**不完全相同**的工作。

## 5. Candidate conversation prompts | 候选人沟通问题

1. 你参与的是 image/video foundation pre-training，还是 fine-tuning、inference 或应用层？
2. 你具体负责模型结构、损失函数、训练数据、分布式系统或模型评估中的哪部分？
3. 视频方向主要解决时间一致性、运动建模还是高分辨率生成？
4. 有哪些公开论文、报告或代码能够支持你描述的成果？

[Research methodology](../methodology/source-policy.md) · Updated: 2026-11-17
