# 🧠 LLM Foundation Training | 大语言模型基座训练

> A research-and-talent lens on how foundation language models are trained.  
> 这份笔记聚焦**基座预训练**；不要把预训练与后训练、推理服务或 Agent 应用混为一谈。

[← Back to Radar](../README.md)

## 1. What is foundation pre-training? | 什么是基座预训练？

基座预训练通常指模型在大规模语料和算力支持下，学习通用语言或多模态表示与生成能力的阶段。对自回归语言模型而言，常见目标是**预测下一个 token**；不同体系也可能采用其他目标。

一个简化视角：

**数据采集与治理 → Tokenizer / 数据混配 → 模型架构与训练目标 → 分布式训练 → Checkpoint 与评估 → 后续后训练及部署。**

预训练并非单纯“堆 GPU”：数据质量、token 分布、训练稳定性、实验设计、故障恢复和客观评估都会影响模型质量与研发效率。

## 2. Five technical questions | 五个追踪维度

| 维度 | 关键问题 | 常见岗位协作 |
| --- | --- | --- |
| **Architecture** | 模型结构、注意力机制、参数规模或专家结构如何取舍？ | Base-model research, model architecture |
| **Data** | 语料如何清洗、去重、过滤、混配并控制污染？ | Pre-training data, data platform |
| **Scaling** | 在固定算力预算下，参数量与训练 token 怎样配置？ | Pre-training research, training strategy |
| **Training systems** | 并行策略、混合精度、通信、吞吐和稳定性如何优化？ | Training systems, distributed systems |
| **Evaluation** | 能力、鲁棒性、泛化、数据污染与训练曲线怎样追踪？ | Evaluation, model research |

## 3. Foundational reading | 经典文献入口

| Paper | Why it matters | Source |
| --- | --- | --- |
| **Attention Is All You Need** (2017) | Transformer 架构研究的经典基础文献 | [Vaswani et al.](https://arxiv.org/abs/1706.03762) |
| **Language Models are Few-Shot Learners** (2020) | 大规模自回归语言模型与上下文学习的重要研究 | [Brown et al.](https://arxiv.org/abs/2005.14165) |
| **Training Compute-Optimal Large Language Models** (2022) | 探讨训练算力预算下模型规模与训练 token 配比 | [Hoffmann et al.](https://arxiv.org/abs/2203.15556) |

这里的“经典”指**理解研究路线的起点**，不代表这些论文对 2026 年最新模型或岗位提供了完整描述。

## 4. From research to talent | 从技术问题到人才画像

- **预训练研究员**：关注建模假设、数据与算力实验、scaling 规律、训练结果解释。
- **预训练数据研究 / 工程**：关注高质量语料、数据过滤、配比、去重、数据质量评估。
- **训练系统工程师**：关注大规模分布式训练、并行、性能瓶颈、稳定性、checkpoint。
- **模型评估研究 / 工程**：关注基准设计、数据泄漏、训练中评估和误差归因。

**重要提醒**：这些是工作方向，不是绝对独立的岗位名称。同一位研究员可能负责多个环节；团队规模不同，岗位边界也不同。

## 5. Questions worth asking | 人才沟通时的核验问题

1. 你主要参与预训练链路中的哪一步？哪些是你亲自负责的？
2. 你负责的是模型实验、数据策略，还是训练系统与性能？
3. 做过哪些可公开描述的实验设计、故障定位或评估方案？
4. 你如何判断模型改进来自架构、数据、算力还是实验因素？
5. 有哪些已公开的论文、技术报告或代码可用于佐证贡献？

*避免索取候选人受保密义务约束的训练数据、内部超参、未发布模型细节或公司机密。*

## 6. Notes to expand

- Mixture-of-Experts 的训练取舍
- 长上下文与训练稳定性
- 训练数据的质量评估和污染控制
- 大规模训练通信、并行和容错

[Research methodology](../methodology/source-policy.md) · Updated: 2026-11-17
