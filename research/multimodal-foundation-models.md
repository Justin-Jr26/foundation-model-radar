# 👁️ Multimodal Foundation Models | 多模态基座模型

> From separate representations to models that learn across modalities.  
> 聚焦图像、视频、音频与语言的**基础表征、联合训练和跨模态建模**。

[← Back to Radar](../README.md)

## 1. Core idea | 核心概念

多模态模型研究的是如何让模型学习、理解或生成不同模态的信息。常见研究问题包括：

- **跨模态表征**：图像、文本或音频怎样进入可比较或可融合的表示空间？
- **融合与对齐**：不同模态如何结合、保持语义对应，并处理时序信息？
- **训练数据**：图文、视频文本、语音文本等配对数据如何采集、筛选、标注和评估？
- **目标与评测**：对比学习、自回归生成、感知任务等训练目标如何影响能力？

“多模态”是宽泛技术分类，**CLIP、视觉语言助手、视频生成基础模型**并不拥有完全相同的训练目标和岗位画像。

## 2. Representative research routes | 三类研究路线

| 路线 | 典型问题 | 人才观察维度 |
| --- | --- | --- |
| **Cross-modal contrastive learning** | 如何用图文对建立跨模态表示？ | Representation learning, data curation |
| **Vision-language modeling** | 如何把视觉输入接入语言生成和推理系统？ | Multimodal alignment, model architecture |
| **Temporal / video modeling** | 如何处理连续帧、时间一致性与长序列信息？ | Video understanding, temporal modeling, training systems |

## 3. Foundational reading | 经典文献

- **CLIP — Learning Transferable Visual Models From Natural Language Supervision** (2021)：文本与视觉的对比式预训练及零样本迁移研究。[Paper](https://arxiv.org/abs/2103.00020)
- **Flamingo — a Visual Language Model for Few-Shot Learning** (2022)：视觉与语言模型结合的研究路线之一。[Paper](https://arxiv.org/abs/2204.14198)
- **Visual Instruction Tuning / LLaVA** (2023)：视觉语言模型与指令微调的典型工作；**注意其指令微调环节不等同于从零基座预训练**。[Paper](https://arxiv.org/abs/2304.08485)

## 4. Role map | 相关人才画像

**多模态基础研究**：编码器、跨模态融合、训练目标、视频或音频表征。  
**多模态数据研究 / 工程**：数据配对、质量打分、数据采样、标注和过滤。  
**多模态训练系统**：高分辨率、多帧序列带来的显存、吞吐、存储和通信问题。  
**多模态评估**：感知、理解、生成质量、长视频时序一致性以及数据污染。

## 5. Talent screening | 分辨真实参与深度

- 负责**基础表征学习**还是在已有模型上做微调、指令对齐与应用？
- 自己设计过哪些模型、训练目标或数据实验？
- 如果做视频，重点是视频**理解**还是视频**生成**？
- 处理过哪些公开可描述的数据质量、时序对齐或训练稳定性问题？

同样的“Multimodal”标签可能对应差异巨大的岗位，不能仅凭关键词判断匹配度。

## 6. Upcoming notes

- Unified multimodal foundation training
- Audio-language and video-language learning
- Video foundation-model data pipelines

[Research methodology](../methodology/source-policy.md) · Updated: 2026-11-17
