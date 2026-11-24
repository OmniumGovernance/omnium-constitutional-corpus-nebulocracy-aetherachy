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

A large-scale, structured high concept level theoretical-governance and constitutional worldbuilding dataset in English, packaged in **Apache Parquet**, **JSONL (UTF-8)**, and **PDF** formats for **long-context NLP**, **retrieval-augmented generation (RAG)**, **hierarchical document parsing**, and **language model pretraining**.

Nebulocracy Aetherarchy: The Supreme Constitution (Omnium Edition v2) is a monumental, 3.32-million-word (~8,608-page / ~11,879-Article) master constitutional codex, philosophical treatise, and complete sovereign civilization blueprint. Building upon the foundational framework originally conceived by theoretical physicist Daniel Kasper and originally licensed under CC0 1.0, this Omnium v2 edition—developed and expanded by OmniumGovernance—scales the architecture into a comprehensive, nine-rank, 66-branch polycentric governance operating system.

Designed simultaneously as a next-generation blueprint for human governance and a high-density, structured reasoning corpus for Artificial General Intelligence (AGI) alignment, Constitutional AI, and long-context LLM training, this work codifies an entire post-scarcity, self-correcting society from first principles down to local municipal administration.

Key Architectural & Institutional Details:

Nine-Rank Polycentric Holarchy (Ranks 0–8): Organizes constitutional foundations, supreme guardianship, polycentric branches, truth and ethics anchor parliaments, fractal coordination, specialized agencies, eight-tier territorial governance (Global down to Village), operational institutions, and non-sovereign technical/AI infrastructure under the principle of unity without institutional uniformity and cooperation without absorption.
66 Co-Equal Omni Branches: Distributes domain-specific legislative, executive, and internal adjudicative authority across 66 autonomous branches—covering theoretical physics, ecological renewal, longevity, anti-corruption, psychological resilience, aesthetic architecture, and hyperintelligence—each with its own branch parliament, immediate-action executive house, and research apparatus.
Multi-Level Territorial & Legal Design: Pairs Swiss-inspired cantonal autonomy and eight-level territorial scaling (up to a 528-complex planning framework) with Finnish-inspired fundamental rights, rule of law, and mandatory governance education and recertification for public officials.
Recursive Simulation & AGI Safeguards: Incorporates three recursive policy-validation cycles (Empirical Feasibility Testing, Ethical and Legal Resilience Modeling, and Strategic Stability Simulation) across OSMRPTDZ simulator centres, alongside strict Technical Non-Sovereignty firewalls ensuring AI, surveillance, and data systems remain support infrastructure subordinate to human rights and due process.

Reading & Research Utility:

​Structured for both human reading and automated ingestion, featuring numbered chapters, articles, ranks, institutional registers, and cross-referenced governance mandates. Most readers are not going to sit down and read 8,000+ pages from cover to cover—instead, you can load the constitution into Gemini, ChatGPT, or another capable AI model and have the AI explain, summarize, and answer questions about it for you.

​Suited for Constitutional AI and value-alignment research, multi-hop legal and institutional reasoning, and ultra-long-context LLM evaluation across millions of words of interconnected normative and structural text.

​"Through Reason, Unity; Through Unity, Flourishing."

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
* **High Concept Level Theoretical-Governance & Worldbuilding:** Studying large-scale fictional constitutional and institutional frameworks.

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
