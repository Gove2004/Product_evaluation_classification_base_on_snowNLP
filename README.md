# 基于SnowNLP的商品评价分类模型

## 项目简介

本项目是一个基于SnowNLP的中文商品评价情感分类系统，能够自动将商品评论分类为"负面"、"中性"或"正面"三类。项目旨在为电商平台提供自动化的用户反馈分析工具，帮助商家快速了解消费者对产品的评价。

## 主要功能

- **情感分类**：使用SnowNLP对商品评论进行情感分析
- **批量处理**：支持批量处理大量评论数据
- **自定义规则**：结合关键词匹配优化基础模型结果
- **结果可视化**：提供分类结果的统计展示

## 技术特点

- 基于Python 3.x开发
- 使用SnowNLP作为核心情感分析引擎
- 通过关键词匹配和规则优化提高分类准确率
- 模块化设计，便于扩展和集成

## 文件结构

```
Product_evaluation_classification_base_on_snowNLP/
├── batch_processor.py      # 批量处理脚本
├── snownlp_analyzer.py     # 核心分析模块
└── README.md               # 项目说明文档
```

## 安装与使用

### 依赖安装

```bash
pip install snownlp
```

### 快速开始

1. 克隆本项目：
```bash
git clone https://github.com/Gove2004/Product_evaluation_classification_base_on_snowNLP.git
```

2. 运行示例分析：
```python
from snownlp_analyzer import predict_sentiment

result = predict_sentiment("这个产品质量很好，但物流太慢了")
print(result)
```

3. 批量处理评论文件：
```bash
python batch_processor.py input.txt output.csv
```

## 性能说明

当前模型在测试集上的准确率约为75%-80%，对于特定领域的商品评论，建议：

1. 收集领域相关数据
2. 重新训练SnowNLP的情感分析模型
3. 调整关键词和规则设置

## 贡献指南

欢迎通过Pull Request提交改进：
- 优化分类规则
- 添加新的预处理方法
- 提高批量处理效率

## 许可证

本项目采用MIT开源许可证。

## 联系方式

如有问题或建议，请联系项目维护者
