# Semantic Resume–Job Matching with Sentence-BERT

This project explores semantic matching between resumes and job postings using a fine-tuned Sentence-BERT bi-encoder.

Starting from a pretrained SBERT model, we generate pseudo-labels via embedding similarity and word-level heuristics, and fine-tune all transformer layers using a contrastive loss. The resulting model learns task-specific representations that better align candidate skills with job requirements compared to a frozen baseline.

**Key components**
- Sentence-BERT bi-encoder architecture
- Pseudo-labelling based on embedding proximity and keyword overlap
- Contrastive fine-tuning for binary relevance classification
- Embedding-space evaluation and visualisation

**Data**
Publicly available Kaggle datasets of resumes and job postings.

This repository contains the full Jupyter notebook used for data processing, model training, and evaluation.
