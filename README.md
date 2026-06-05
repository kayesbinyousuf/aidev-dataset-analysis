# AIDev Dataset Analysis

**Author:** [Kayes Bin Yousuf](https://linkedin.com/in/kayes-bin-yousuf) — ML Researcher | Renewable Energy & Industrial AI | Reviewer @Elsevier

Advanced NLP-based consistency analysis of AI development pull requests using TF-IDF vectorization, cosine similarity, and Latent Dirichlet Allocation (LDA) topic modelling.

---

## Overview

This tool analyzes pull request datasets from AI development repositories to measure **description–diff consistency** — the degree to which a PR's textual description matches the actual code changes. It processes large datasets in a memory-efficient streaming fashion and produces visualizations of consistency distributions, topic clusters, and agent-level breakdowns.

---

## Key Features

- **TF-IDF + Cosine Similarity** — measures semantic alignment between PR title/description and code diff text
- **LDA Topic Modelling** — discovers latent topics across PR descriptions
- **Memory-efficient streaming** — chunked processing with `psutil` monitoring, suitable for large HuggingFace datasets
- **Agent-level breakdown** — consistency scores grouped by contributing agent/user
- **Visualizations** — consistency score distributions, topic distributions, per-agent comparisons

---

## How to Run

### Option 1 — Google Colab (Recommended)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1GFFy8-hCmyVT-X0bXIt0dG2cOKuplgMq#scrollTo=CiRpDF3AEZiE)

### Option 2 — Local

```bash
git clone https://github.com/kayesbinyousuf/aidev-dataset-analysis.git
cd aidev-dataset-analysis
pip install -r requirements.txt
python aidev_analyzer.py
```

---

## Dependencies

```
datasets>=2.14.0
scikit-learn>=1.3.0
nltk>=3.8
numpy>=1.24.0
pandas>=2.0.0
matplotlib>=3.7.0
tqdm>=4.65.0
psutil>=5.9.0
```

---

## Repository Structure

```
aidev-dataset-analysis/
├── aidev_analyzer.py   # Main analysis script
├── requirements.txt
├── LICENSE
└── README.md
```

---

## License

[MIT License](LICENSE)
