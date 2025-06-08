# -# DetectiveMOE: 侦探推理混合专家系统

## 项目概述

DetectiveMOE 是一个基于混合专家模型(Mixture of Experts)的侦探推理系统，能够分析案件描述、证据线索和嫌疑人信息，进行逻辑推理、证据验证和动机分析，最终生成推理报告和证据知识图谱。

## 文件结构
detective_moe/
├── detective_moe.py  # 核心模型实现
├── inference_example.py # 推理示例
├── train_detective_moe.py # 模型训练脚本
└── README.md # 项目说明文档
## 重要代码模块
- LogicExpert
- EvidenceValidationExpert
- MotiveAnalysisExpert
- GatedNetwork
- inference
- DetectiveMOE
## 安装需求
pip install torch transformers networkx
## 输出示例
==================================================
侦探推理系统结果
==================================================

案件置信度: 0.87/1.00
主要推理方式: 溯因推理
关键证据可信度: 0.92
证据间矛盾程度: 0.15
嫌疑人动机强度: 0.78

专家贡献权重:
- 逻辑推理专家: 0.35
- 证据校验专家: 0.45
- 动机推理专家: 0.20

知识图谱数据已保存至 evidence_graph.json
## 目前还未完成
- 目前还没有完成复杂长文本生成推理链条任务
- 专家系统的专家目前只有三个还不够多
- 目前串行结构还没有完全应用跑通，目前代码只是三个专家分开自己干自己的活
- 专家还不够特殊化，未接入相关领域模块加强
