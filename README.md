# POS Tagging and Chunking with BERT

This repository contains a token classification pipeline using BERT for POS tagging and chunking. The project demonstrates the end-to-end workflow: dataset handling, preprocessing, model training, evaluation, and inference.

Datasets Used
- POS Tagging:[Treebank dataset](https://huggingface.co/datasets/treebank)
- Chunking: [CoNLL-2000 dataset](https://huggingface.co/datasets/conll2000)

Pipeline Overview
1. Data Loading: Load POS and chunking datasets using Hugging Face `datasets`.
2. Preprocessing:
   - Tokenization with `BERT tokenizer`
   - Label alignment for subwords
3. Model Setup: `AutoModelForTokenClassification` from Hugging Face Transformers
4. Training:   Fine-tune BERT on POS and chunk datasets
5. Evaluation: Compute Precision, Recall, F1 Score using `seqeval`
6. Inference:  Predict POS and chunk tags for custom sentences
7. Comparison: Highlight differences between POS tagging and chunking

Requirements
- Python 3.10+
- Hugging Face Transformers
- Datasets
- Seqeval
- PyTorch

