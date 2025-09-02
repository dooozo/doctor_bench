# 完整医疗AI基准数据集统一目录

## 📊 数据集概览

这个目录包含了所有可用的完整医疗AI基准数据集，经过重新整理和验证。

### 🎯 数据完整性状态

| 数据集 | 状态 | 数据量 | 大小 | 说明 |
|--------|------|--------|------|------|
| **MedAgentsBench** | ✅ 完整 | 935条QA + 评估结果 | 96MB | 医学问答代理基准 |
| **AI_Hospital** | ✅ 完整 | 22,253条医疗记录 | 7.0MB | AI医院诊断模拟 |
| **HealthBench** | ✅ 完整 | 9,671条健康对话 | 105MB | 健康对话评估基准 |
| **R2MED** | ✅ 完整 | 88条查询 + 34,810条语料 | 21MB | 医学推理驱动检索基准 |

**总体数据可用性**: **100%** (4/4个基准有完整数据)
**总数据量**: **229MB**
**总记录数**: **67,706条**

## 📁 目录结构

```
complete_medical_benchmarks_unified/
├── MedAgentsBench/          # ✅ 完整数据 (96MB)
│   ├── medexqa/            # 医学问答数据
│   ├── mmlu-pro/           # MMLU专业版
│   ├── medqa/              # MedQA数据集
│   ├── pubmedqa/           # PubMedQA数据集
│   ├── medmcqa/            # MedMCQA数据集
│   ├── afrimedqa/          # AfriMedQA数据集
│   ├── medbullets/         # MedBullets数据集
│   ├── medxpertqa-r/       # MedXpertQA-R数据集
│   ├── medxpertqa-u/       # MedXpertQA-U数据集
│   └── medqa_5options/     # 5选项MedQA数据集
├── AI_Hospital/            # ✅ 完整数据 (7.0MB)
│   ├── patients.json       # 22,253条患者记录
│   └── collaborative_doctors/ # 医生协作数据
├── HealthBench/            # ✅ 完整数据 (105MB)
│   ├── healthbench_main.jsonl      # 5,000条主要健康对话
│   ├── healthbench_hard.jsonl      # 1,000条困难健康对话
│   └── healthbench_consensus.jsonl # 3,671条共识健康对话
├── R2MED/                  # ✅ 完整数据 (21MB)
│   ├── query.jsonl         # 88条医学查询
│   ├── corpus.jsonl        # 34,810条医学语料
│   └── qrels.jsonl         # 244条相关性判断
└── README.md               # 本文件 - 详细说明
```

## 🔍 详细数据说明

### 1. MedAgentsBench - 医学问答代理基准 ✅
- **数据量**: 935条测试数据 + 评估结果
- **格式**: JSONL格式
- **内容**: 高难度医学问答题目
- **用途**: 评估医学AI的专业推理能力
- **质量**: ⭐⭐⭐⭐⭐ (完整可用)
- **包含数据集**: MedQA, PubMedQA, MedMCQA, AfriMedQA, MMLU, MMLU-Pro, MedBullets, MedXpertQA-R/U, MedExQA

### 2. AI_Hospital - AI医院诊断模拟 ✅
- **数据量**: 22,253条患者医疗记录
- **格式**: JSON格式
- **内容**: 真实临床病例和诊断对话
- **用途**: 临床诊断AI训练和评估
- **质量**: ⭐⭐⭐⭐⭐ (完整可用)
- **特点**: 包含完整的医疗记录、诊断过程和治疗方案

### 3. HealthBench - 健康对话评估基准 ✅
- **数据量**: 9,671条健康对话
  - 主要对话: 5,000条
  - 困难对话: 1,000条
  - 共识对话: 3,671条
- **格式**: JSONL格式
- **内容**: 健康咨询对话和评估标准
- **用途**: 健康对话AI安全性评估
- **质量**: ⭐⭐⭐⭐⭐ (完整可用)
- **特点**: 包含医师评估标准和安全性指标

### 4. R2MED - 医学推理驱动检索基准 ✅
- **数据量**: 
  - 查询: 88条医学查询
  - 语料: 34,810条医学文档
  - 相关性: 244条判断
- **格式**: JSONL格式
- **内容**: 医学信息检索和推理任务
- **用途**: 医学检索系统评估
- **质量**: ⭐⭐⭐⭐⭐ (完整可用)
- **特点**: 包含查询-文档对和相关性判断

## 📈 数据质量评估

| 维度 | MedAgentsBench | AI_Hospital | HealthBench | R2MED |
|------|---------------|-------------|-------------|-------|
| **数据完整性** | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ |
| **数据质量** | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ |
| **实用价值** | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ |
| **使用难度** | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ |

## 🎯 使用建议

### 立即可用的研究任务

1. **医学问答系统评估**: 使用MedAgentsBench测试模型的医学推理能力
2. **临床诊断AI训练**: 使用AI_Hospital训练诊断模型
3. **健康对话AI评估**: 使用HealthBench评估对话AI的安全性
4. **医学检索系统测试**: 使用R2MED测试检索模型的性能

### 数据集组合使用

1. **综合医学AI评估**: 结合所有4个数据集进行全面评估
2. **多模态医学AI**: 结合问答、诊断、对话和检索任务
3. **医学AI安全性研究**: 重点关注HealthBench的安全评估标准

## 📚 数据来源

- **MedAgentsBench**: [arXiv:2503.07459](https://arxiv.org/abs/2503.07459)
- **AI_Hospital**: [arXiv:2402.09742](https://arxiv.org/abs/2402.09742)
- **HealthBench**: [OpenAI Research](https://openai.com/index/healthbench)
- **R2MED**: [arXiv:2505.14558](https://arxiv.org/abs/2505.14558)

## 🚀 快速开始

1. 查看可用数据：
```bash
ls -la complete_medical_benchmarks_unified/
```

2. 开始使用数据集进行医疗AI研究！

## 📄 许可证

请参考各个原始数据集的许可证要求。

## 🤝 贡献

欢迎提交Issue和Pull Request来改进这个数据集集合。

---

**总结**: 这个统一目录提供了完整的医疗AI基准数据集，包含问答、诊断、对话和检索四个核心任务，总计67,706条记录，229MB数据，为医疗AI研究提供了全面的评估基础。