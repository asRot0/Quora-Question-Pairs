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

## 📌 Understanding TF-IDF in NLP

## 🔍 TF-IDF Formula Breakdown  
The **TF-IDF (Term Frequency-Inverse Document Frequency)** score for a word **W** in a document **D** is computed as:

\[
\text{TF-IDF}(W, D) = \text{TF}(W, D) \times \text{IDF}(W)
\]

Where:  
- **TF (Term Frequency)** = How often word **W** appears in **D**.  
- **IDF (Inverse Document Frequency)** = Measures how rare **W** is across **all documents**.  

\[
\text{IDF}(W) = \log \left( \frac{\text{Total Documents}}{\text{Number of Documents Containing } W} \right)
\]

📌 **If a word appears in almost every document, its IDF score is low** → **Less Important**  
📌 **If a word is unique to a few documents, its IDF score is high** → **More Important**  

---

## 🚀 Example of TF-IDF Importance  
### **Dataset: Three Documents**
1️⃣ **"The movie was amazing and had great cinematography."**  
2️⃣ **"The cinematography and plot twist were Oscar-worthy!"**  
3️⃣ **"I love this movie, but the ending was bad."**  

| **Word**           | **TF-IDF Score** | **Importance** |
|------------------|-----------------|--------------|
| **cinematography** | High            | ✅ Important (Rare, specific to some documents) |
| **plot twist**     | High            | ✅ Important (Key phrase in only one document) |
| **movie**          | Low             | ❌ Less Important (Appears in all documents) |
| **the, was, and**  | Very Low        | ❌ Stopwords, common in all text |

---

## 📈 Why Use TF-IDF?  
🚀 **TF-IDF improves text representation** by **reducing the impact of common words** while **giving importance to unique words**.  
💡 **This is crucial in NLP tasks** like **text classification, document similarity, and search engines**.  

---

## 🛠️ Use Cases  
- **Question Deduplication**: Helps in reducing redundant questions in Q&A platforms.  
- **Semantic Text Similarity**: Improves chatbot and search engine performance.  
- **NLP Model Training**: Can be used to train models for text similarity tasks.

---
🔹 **Note:** This dataset is provided by Quora and is publicly available for research and learning purposes.
