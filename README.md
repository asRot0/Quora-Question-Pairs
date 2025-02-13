# Quora Question Pairs - Dataset Overview

## 📌 Dataset Description  
The **Quora Question Pairs** dataset aims to identify whether two questions asked on Quora are **duplicate** or not. This is a classic **natural language processing (NLP) problem** where the goal is to improve the **question-answering system** by detecting similar intent in different wordings.

## 📂 Dataset Files  
The dataset contains the following files:  

| File Name                | Description |
|--------------------------|-------------|
| `train.csv.zip`          | Training dataset (contains question pairs and labels) |
| `test.csv.zip`           | Test dataset (without labels, used for evaluation) |
| `sample_submission.csv.zip` | Sample format for submission |

## 📊 Data Fields  
Each row in the dataset represents a pair of questions with the following columns:  

| Column Name   | Description |
|--------------|-------------|
| `id`         | Unique identifier for the row |
| `qid1`       | Unique ID for question 1 |
| `qid2`       | Unique ID for question 2 |
| `question1`  | First question in the pair |
| `question2`  | Second question in the pair |
| `is_duplicate` | **Label (Target Variable):** 1 if questions are duplicates, 0 otherwise |

## 📈 Dataset Statistics  
- **Total Rows:** 404,290  
- **Duplicate Questions:** ~37%  
- **Unique Questions:** 537,933  

## 🔗 Dataset Source  
The dataset is part of the **Quora Question Pairs** competition on Kaggle:  
[🔗 Kaggle Dataset](https://www.kaggle.com/competitions/quora-question-pairs/data)

## 🛠️ Use Cases  
- **Question Deduplication**: Helps in reducing redundant questions in Q&A platforms.  
- **Semantic Text Similarity**: Improves chatbot and search engine performance.  
- **NLP Model Training**: Can be used to train models for text similarity tasks.

---
🔹 **Note:** This dataset is provided by Quora and is publicly available for research and learning purposes.
