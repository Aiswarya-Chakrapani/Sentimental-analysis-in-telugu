# 📊 Telugu Sentiment Analysis – A Comparative Study of Algorithms

This project performs **sentiment analysis** on Telugu text using both traditional machine learning and deep learning models. The goal is to evaluate and compare the performance of various algorithms in handling sentiment classification in a **low-resource language** like Telugu.

---

## 🧠 Abstract

Sentiment analysis in regional languages like Telugu presents challenges due to **limited datasets** and **complex linguistic structures**. This project compares the effectiveness of **seven algorithms**: Logistic Regression, Linear SVM, Decision Tree, Random Forest, LSTM, CNN, and BERT. 

The results highlight that **LSTM** performs the best due to its ability to capture word-order dependencies in Telugu, while **BERT underperformed**, likely due to insufficient pretraining for the Telugu language.

---

## 📚 Dataset Overview

- **Source**: Telugu text from social media and public datasets
- **Train samples**: 23,800  
- **Test samples**: 6,806  
- **Class Distribution**:
  - Positive: 27%
  - Negative: 19%
  - Neutral: 53%

---

## 🧹 Preprocessing Steps

1. Removed non-Telugu characters
2. Handled missing values
3. Removed duplicates
4. Encoded sentiment labels:
   - Positive → `1`
   - Negative → `-1`
   - Neutral → `0`

---

## 🧪 Feature Engineering

- **TF-IDF Vectorization**
- **Min-Max Scaling**
- **Top Keywords**:
  - "బాగుంది" (good)
  - "చెడ్డది" (bad)
  - "సరదాగా" (fun)

---

## 🤖 Models Compared

### 🔸 Machine Learning Models:
- **Logistic Regression** – Baseline model, 58.99% accuracy
- **Linear SVM (SGD)** – Similar performance, 58.58% accuracy
- **Decision Tree** – 51% accuracy; struggles with agglutinative nature of Telugu
- **Random Forest** – 54.5% accuracy

### 🔸 Deep Learning Models:
- **LSTM** – Best performing model, **61.43% accuracy**
- **CNN** – Underperformed, 52% accuracy

### 🔸 Transformer Model:
- **BERT** – 54.31% accuracy; shows limitations of transfer learning in low-resource languages

---

## 📊 Results Summary

| Algorithm       | Accuracy |
|----------------|----------|
| Logistic Regression | 58.99% |
| Linear SVM          | 58.58% |
| Decision Tree       | 51.00% |
| Random Forest       | 54.50% |
| CNN                 | 52.00% |
| **LSTM**            | **61.43%** |
| BERT                | 54.31% |

LSTM clearly outperforms due to its ability to model sequence and context effectively in Telugu.

---

## 📈 Visuals

The project includes:
- Sentence Length Histograms
- Sentiment Label Distributions
- Top 20 Frequent Words
- Accuracy/Recall Charts

---


## 🔚 Conclusion

This study provides critical insight into the **efficacy of various algorithms** for sentiment analysis in Telugu. LSTM is most effective, while models like BERT show potential with better language-specific pretraining.

---

