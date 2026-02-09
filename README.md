English | [简体中文](./README_CN.md)
# FinRAG: A Chinese Financial Event Knowledge Graph-Based Retrieval-Augmented Generation Framework for Financial Question Answering

![GitHub](https://img.shields.io/github/license/chtkg/FinRAG)
![GitHub last commit](https://img.shields.io/github/last-commit/chtkg/FinRAG)

## Overall Framework
FinRAG, a Retrieval-Augmented Generation framework based on a Chinese financial event knowledge graph(see Fig.1). The framework first combines semantic-aware chunking and large language model(LLM)-based triplet extraction to construct a structured index, which enhances retrieval efficiency and supports accurate financial event reasoning. The framework incorporates a generation-verification process to ensure reliable and relevant information retrieval. Then, a query reconstruction module based on reinforcement learning is designed to convert vague user queries into domain-specific expressions, significantly improving intent recognition accuracy. 
Finally, we design a dual-level retrieval mechanism inspired by LightRAG, and adapt it to the financial domain. The first level retrieves core entities based on semantic similarity, while the second level completes event chains through knowledge graph–based neighbor expansion.
Experimental results demonstrate that the proposed framework outperforms general RAG baselines on a self-constructed Chinese financial question answering dataset.

<p align="center">
  <img src="./figure1.png" width="600"/>
</p>
<p align="center">
Figure 1: Overview of the FinRAG framework.
</p>

## Key Features

- 🏦 **Domain-Specialized** - Optimized for complex Chinese financial terminology and multi-source data
- 🧠 **Knowledge Graph Integration** - Combines 1,200 professional research reports with structured event knowledge
- 🔍 **Dual-Level Retrieval** - Semantic similarity search + knowledge graph expansion
- ✅ **Generation-Verification** - Ensures reliable outputs through link prediction
- 🚀 **Query Reconstruction** - RL-based transformation of vague queries into domain-specific expressions

## Dataset

| Component | Quantity | Content Types |
|-----------|----------|---------------|
| Research Reports | 1,200 | Company analyses, Industry research, Macroeconomic evaluations |
| QA Pairs | 3,600 | Single-hop, Multi-hop, Open-ended questions |

All content curated by financial experts and knowledge graph engineers.

## Quick Start

### Installation

```bash
git clone https://github.com/chtkg/FinRAG.git
cd FinRAG

