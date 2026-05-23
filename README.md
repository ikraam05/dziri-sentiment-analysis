# Algerian Dialect Sentiment Analysis using DziriBERT

This project focuses on sentiment analysis for Algerian dialect (Darija) tweets using the Twifil dataset and DziriBERT transformer model.

---

# Project Objectives

- Analyze Algerian dialect tweets
- Perform dialect-specific preprocessing
- Fine-tune DziriBERT for sentiment classification
- Compare balancing strategies:
  - SMOTE
  - ADASYN
  - back transaction
  - Focal Loss
  - class weighting
  - focal loss + class weighting
  - focal loss + back transaction


# Dataset

Dataset used:
Twifil Dataset

Contains:
- Algerian dialect tweets
- Arabic
- French
- Arabizi
- Code-switching



# Model

Base model:
DziriBERT

# Evaluation Metrics
Accuracy
F1-score
F1-macro
Recall
G-Mean
Confusion Matrix


# Main Results
Model	           F1-Macro
Baseline         0.68
SMOTE       	   0.64
Focal Loss   	   0.68

# Main observation:
Advanced balancing methods did not significantly improve performance due to the linguistic complexity of Algerian dialect and ambiguity of Neutral tweets.

# Technologies Used
Transformers
HuggingFace
Scikit-learn
PyTorch
Matplotlib
Seaborn


# Author
Ikram Yadel



#  requirements.txt

transformers
datasets
torch
scikit-learn
imbalanced-learn
pandas
numpy
matplotlib
seaborn
wordcloud
emoji
