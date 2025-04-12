# SkimLit: Research Paper Classifier using NLP and TensorFlow

This project, **SkimLit**, is an NLP milestone project where a deep learning model is trained to classify sentences from medical research abstracts into their respective parts (e.g., Background, Methods, Results, Conclusions).

## Table of Contents
- [Overview](#overview)
- [Technologies](#technologies)
- [Dataset](#dataset)
- [Approach](#approach)
- [Model Architecture](#model-architecture)
- [Installation](#installation)
- [Usage](#usage)
- [Evaluation](#evaluation)
- [License](#license)

## Overview
The goal of SkimLit is to help researchers automatically identify key sections of scientific abstracts. The model learns to classify sentences into predefined classes using deep learning and NLP techniques.

## Technologies
- Python
- TensorFlow & Keras
- GloVe Embeddings
- NLP Techniques (Tokenization, Padding, Text Vectorization)

## Dataset
The dataset comes from the PubMed 200k RCT (Randomized Controlled Trial) dataset, consisting of thousands of labeled abstracts from medical research papers. Each sentence is labeled as one of:
- OBJECTIVE
- BACKGROUND
- METHODS
- RESULTS
- CONCLUSIONS

## Approach
- Loaded and cleaned the PubMed RCT dataset.
- Preprocessed text: lowercasing, punctuation handling, tokenization.
- Converted words to sequences using pretrained GloVe embeddings.
- Padded and batched sentences for model input.
- Built and trained an RNN-based model using TensorFlow.
- Evaluated performance using accuracy and F1-score.

## Model Architecture
- Embedding Layer (with GloVe vectors)
- Bidirectional LSTM
- Dense output layer with softmax activation

## Installation
```bash
git clone https://github.com/muaazshoaib/skimlit.git
cd skimlit-nlp
pip install -r requirements.txt
