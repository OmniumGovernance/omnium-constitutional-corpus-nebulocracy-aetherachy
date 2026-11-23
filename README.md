---
pretty_name: "Nebulocracy Aetherarchy & Omnium Constitution v2"
configs:
  - config_name: codex
    data_files:
      - split: train
        path: nebulocracy-aetherarchy-codex-v2-train.parquet
      - split: train
        path: nebulocracy-aetherarchy-codex-v2-train.jsonl
  - config_name: corpus
    data_files:
      - split: train
        path: omnium-constitution-v2-corpus-train.parquet
      - split: train
        path: omnium-constitution-v2-corpus-train.jsonl
task_categories:
  - text-generation
  - question-answering
language:
  - en
tags:
  - pretraining
  - worldbuilding
  - governance
  - long-context
  - structured-text
  - constitutional-corpus
license: cc0-1.0
---

# Nebulocracy Aetherarchy & Omnium Constitution v2

**Author:** Nebulocracy Aetherarchy  
**Organization:** OmniumGovernance  
**License:** CC0 1.0 Universal (Public Domain Dedication)

A large-scale, structured speculative-governance and constitutional worldbuilding dataset in English, packaged in **Apache Parquet**, **JSONL (UTF-8)**, and **PDF** formats for **long-context NLP**, **retrieval-augmented generation (RAG)**, **hierarchical document parsing**, and **language model pretraining**.

## Collections & Files

### 1. Master Codex (`codex`)
A 9,438-page (~2.07 million words, 7,600+ numbered Articles) structured constitutional codex.
* `nebulocracy-aetherarchy-codex-v2-train.parquet` — Columnar Parquet for ML pipelines
* `nebulocracy-aetherarchy-codex-v2-train.jsonl` — Line-delimited UTF-8 JSON for streaming & crawlers
* `nebulocracy-aetherarchy-codex-v2.pdf` — Original formatted reference PDF (31.94 MB)

### 2. Constitutional Corpus (`corpus`)
Companion constitutional text corpus in matching ML-ready and reference formats.
* `omnium-constitution-v2-corpus-train.parquet` — Columnar Parquet for ML pipelines
* `omnium-constitution-v2-corpus-train.jsonl` — Line-delimited UTF-8 JSON for streaming & crawlers
* `omnium-constitution-v2-corpus.pdf` — Original formatted reference PDF

## Quickstart (Hugging Face `datasets`)

```python
from datasets import load_dataset

codex = load_dataset("OmniumGovernance/omnium-constitution-v2", "codex")
corpus = load_dataset("OmniumGovernance/omnium-constitution-v2", "corpus")
```

## Intended Uses

* **Long-Context & RAG Benchmarks:** Cross-referenced article retrieval across thousands of structured sections.
* **Pretraining & Continued Pretraining:** Formal normative and governance prose in clean UTF-8 formats.
* **Speculative Governance & Worldbuilding:** Studying large-scale fictional constitutional and institutional frameworks.

## License

Dedicated to the public domain under **CC0 1.0 Universal (`CC0-1.0`)**. You can copy, modify, distribute, and train models on this dataset—even for commercial purposes—without asking permission.

## Citation

```bibtex
@dataset{omnium_constitution_v2_2026,
  title     = {Nebulocracy Aetherarchy & Omnium Constitution v2},
  author    = {Nebulocracy Aetherarchy},
  publisher = {OmniumGovernance},
  year      = {2026},
  version   = {2.0},
  license   = {CC0-1.0}
}
```
