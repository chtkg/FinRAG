# FinRAG: A Chinese Financial Event Knowledge Graph-Based Retrieval-Augmented Generation Framework for Financial Question Answering

![GitHub](https://img.shields.io/github/license/chtkg/FinRAG)
![GitHub last commit](https://img.shields.io/github/last-commit/chtkg/FinRAG)


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

