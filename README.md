# Doctor Bench - 医疗AI基准数据集

## 📊 项目简介

这是一个统一的医疗AI基准数据集集合，包含了多个重要的医疗AI评估基准。数据集经过整理和验证，可以直接用于医疗AI模型的研究和评估。

## 🎯 数据集概览

| 数据集 | 状态 | 数据量 | 大小 | 说明 |
|--------|------|--------|------|------|
| **MedAgentsBench** | ✅ 完整 | 935条QA + 评估结果 | 96MB | 医学问答代理基准 |
| **AI_Hospital** | ✅ 完整 | 22,253条医疗记录 | 7.0MB | AI医院诊断模拟 |
| **R2MED_demo** | 🟡 演示版 | 2条查询 | 24KB | 医学检索基准(仅demo) |
| **HealthBench** | 🟡 示例 | 2个对话样例 | 4KB | 健康对话评估(示例) |
| **MedAgentBoard** | ❌ 空 | 0条数据 | 0B | 多代理协作(需运行代码) |
| **R2MED** | ❌ 空 | 0条数据 | 0B | 完整检索数据(下载失败) |

## 📁 目录结构

```
unified_medical_data/
├── MedAgentsBench/          # ✅ 完整数据 (96MB)
│   ├── medexqa/            # 医学问答数据
│   ├── mmlu-pro/           # MMLU专业版
│   └── ...                 # 其他医学QA数据集
├── AI_Hospital/            # ✅ 完整数据 (7.0MB)
│   ├── patients.json       # 22,253条患者记录
│   └── collaborative_doctors/ # 医生协作数据
├── R2MED_demo/             # 🟡 演示数据 (24KB)
│   └── Biology-demo/       # 生物学演示查询
├── HealthBench/            # 🟡 示例数据 (4KB)
│   └── sample_conversations.json # 健康对话样例
├── MedAgentBoard/          # ❌ 空目录
├── R2MED/                  # ❌ 空目录
└── README.md               # 详细说明文档
```

## 🔍 数据集详细说明

### 1. MedAgentsBench - 医学问答代理基准 ✅
- **数据量**: 935条测试数据 + 评估结果
- **格式**: JSONL格式
- **内容**: 高难度医学问答题目
- **用途**: 评估医学AI的专业推理能力
- **质量**: ⭐⭐⭐⭐⭐ (完整可用)

### 2. AI_Hospital - AI医院诊断模拟 ✅
- **数据量**: 22,253条患者医疗记录
- **格式**: JSON格式
- **内容**: 真实临床病例和诊断对话
- **用途**: 临床诊断AI训练和评估
- **质量**: ⭐⭐⭐⭐⭐ (完整可用)

### 3. R2MED_demo - 医学检索基准 🟡
- **数据量**: 2条查询 + 相关文档
- **格式**: JSONL格式
- **内容**: 生物学问题检索样例
- **用途**: 医学信息检索系统评估
- **质量**: ⭐⭐ (仅演示版本)

### 4. HealthBench - 健康对话评估 🟡
- **数据量**: 2个对话样例
- **格式**: JSON格式
- **内容**: 健康咨询对话示例
- **用途**: 健康对话AI安全性评估
- **质量**: ⭐⭐ (仅示例数据)

## 📈 数据可用性统计

- **完整可用**: 2/5 (40%)
- **部分可用**: 2/5 (40%) 
- **完全缺失**: 1/5 (20%)
- **总体数据量**: 23,192条记录
- **总大小**: 103MB

## 🎯 使用建议

### 立即可用的研究任务
1. **医学问答评估**: 使用MedAgentsBench测试模型推理能力
2. **临床诊断训练**: 使用AI_Hospital训练诊断模型
3. **检索系统测试**: 使用R2MED_demo进行初步检索评估

### 需要额外工作的任务
1. **完整检索评估**: 需要获取R2MED完整数据
2. **多代理协作**: 需要运行MedAgentBoard代码
3. **健康对话评估**: 需要生成HealthBench完整数据

## 📚 数据来源

- **MedAgentsBench**: [arXiv:2503.07459](https://arxiv.org/abs/2503.07459)
- **AI_Hospital**: [arXiv:2402.09742](https://arxiv.org/abs/2402.09742)
- **R2MED**: [arXiv:2505.14558](https://arxiv.org/abs/2505.14558)
- **MedAgentBoard**: [arXiv:2505.12371](https://arxiv.org/abs/2505.12371)
- **HealthBench**: OpenAI Research (2025)

## 🚀 快速开始

1. 克隆仓库：
```bash
git clone https://github.com/dooozo/doctor_bench.git
cd doctor_bench
```

2. 查看可用数据：
```bash
ls -la unified_medical_data/
```

3. 开始使用数据集进行医疗AI研究！

## 📄 许可证

请参考各个原始数据集的许可证要求。

## 🤝 贡献

欢迎提交Issue和Pull Request来改进这个数据集集合。

---

**总结**: 这个仓库提供了统一的医疗AI基准数据集，其中MedAgentsBench和AI_Hospital提供了立即可用的完整数据集，其他数据集需要额外的配置或下载步骤。