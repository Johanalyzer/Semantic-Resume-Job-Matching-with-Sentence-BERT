# Resume–Job Matching via Pseudo-Labelled Sentence-BERT Fine-Tuning

This project improves semantic matching between resumes and job postings by fine-tuning Sentence-BERT using high-confidence pseudo-labels.

We first embed all resumes and job descriptions using a pretrained Sentence-BERT model. Candidate pairs are selected based on embedding proximity and further filtered using a word-level keyword overlap heuristic. Pairs that are very close with strong keyword overlap are treated as positive examples, while distant pairs with low overlap form negative examples.

Using these high-confidence positive and negative pairs, we fully fine-tune a Sentence-BERT bi-encoder with contrastive learning. The resulting model learns a task-specific embedding space that places truly matching resumes and job postings closer together than a standard pretrained Sentence-BERT.

**Key ideas**
- Pretrained Sentence-BERT as an embedding baseline
- Pseudo-labelling via embedding similarity + keyword overlap heuristics
- Fine-tuning on high-confidence positives and negatives
- Improved clustering of semantically matching profiles

All experiments and evaluations are contained in the Jupyter notebook.

