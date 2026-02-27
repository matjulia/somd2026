# somd2026
System submission for the SOMD 2026 Shared Task (co-located with NSLP @ LREC 2026).


---

## Overview

This repository contains the code accompanying our system paper:

> *Semantic Centroids and Hierarchical Density-Based Clustering for Cross-Document Software Coreference Resolution: System Description for SOMD 2026*

Our approach combines:
- Sentence-BERT embeddings (`all-MiniLM-L6-v2`)
- FAISS-based KB lookup
- Surface-form normalization & abbreviation resolution 
- HDBSCAN density-based clustering
- Blocking strategy

---

## Repository Structure

```
├── SOMD2026_Subtask1.ipynb   # Pipeline for Subtask 1 & 2 (gold + predicted mentions)
├── SOMD2026_Subtask3.ipynb   # Pipeline for Subtask 3 (large-scale predicted mentions)
└── README.md
```

---

## Requirements

**Python 3.11.7** (conda-forge)

```
sentence-transformers>=2.2.0,<3.0
faiss-cpu>=1.7.0
hdbscan>=0.8.29
scikit-learn>=1.0.0
pandas>=1.3.0
numpy>=1.21.0
tqdm>=4.62.0
matplotlib>=3.4.0
torch>=1.9.0
scipy>=1.7.0
transformers>=4.12.0
tokenizers>=0.10.0
```

---

## Citation

If you use this code, please cite our system paper (citation to be added after proceedings are published).

---

## Shared Task

- **Website:** [SOMD 2026](https://nfdi4ds.github.io/nslp2026/docs/somd_shared_task.html)
- **Workshop:** NSLP 2026 @ LREC 2026 — May 12, 2026
- **Organizers:** SOMD 2026 Shared Task Committee