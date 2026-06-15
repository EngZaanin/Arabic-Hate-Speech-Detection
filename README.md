# Fine-grained Hate Speech Detection in Arabic Text with Linguistic Analysis using Transformers

## Research Paper

The complete research paper is available in:

paper/Fine_Grained_Hate_Speech_Detection_Paper.pdf

## Overview

This project presents a fine-grained hate speech detection system for Arabic text using Transformer-based models. The study focuses on distinguishing between three categories of Arabic social media content:

* Normal
* Abusive
* Hate Speech

The goal is to improve the automatic identification of harmful online content while addressing the linguistic challenges of Arabic, including dialectal variation, spelling inconsistencies, and informal writing styles.

---

## Dataset

The experiments were conducted using the L-HSAB Arabic hate speech dataset.

Dataset classes:

| Class   | Description                                          |
| ------- | ---------------------------------------------------- |
| Normal  | Non-offensive content                                |
| Abusive | Offensive language without explicit hate             |
| Hate    | Explicit hate speech targeting individuals or groups |

---

## Preprocessing

The following preprocessing steps were applied:

* Removal of URLs and user mentions.
* Hashtag normalization.
* Arabic character normalization:

  * أ, إ, آ → ا
  * ؤ → و
  * ئ → ي
  * ى → ي
  * ة → ه
* Reduction of repeated characters.
* Removal of unnecessary symbols and punctuation.
* Text cleaning while preserving important linguistic information.

---

## Methodology

The project follows a Transformer-based approach for Arabic text classification.

Main components:

1. Data preprocessing and normalization.
2. Dataset preparation and train/test splitting.
3. Tokenization using Hugging Face Transformers.
4. Fine-tuning a pre-trained Arabic Transformer model.
5. Model evaluation using standard classification metrics.

---

## Technologies Used

* Python
* PyTorch
* Hugging Face Transformers
* Scikit-learn
* Pandas
* NumPy
* Matplotlib

---

## Evaluation Metrics

The model is evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

---

## Project Structure

```text
Arabic-Hate-Speech-Detection/
│
├── dataset/
│   ├── test.csv
│   └── train.csv
│
├── notebooks/
│   └── NLP_Transformer_Research_Code.ipynb
│
├── results/
│   ├── transformer_only_results.csv
│   └── transformer_error_analysis.csv
│
├── paper/
│   └── Fine_Grained_Hate_Speech_Detection_Paper.pdf
│
├── requirements.txt
└── README.md
```

---

## Installation

```bash
pip install -r requirements.txt
```

---

## Running the Project

Open the notebook:

```bash
jupyter notebook NLP_Transformer_Research_Code.ipynb
```

or run it directly in Google Colab.

---

## Results

The Transformer-based model demonstrates strong performance for Arabic hate speech classification and provides a robust baseline for fine-grained Arabic content moderation.

---

## Future Work

* Explore larger Arabic language models.
* Investigate explainable AI techniques.
* Improve performance on minority classes.
* Incorporate dialect-specific linguistic features.
