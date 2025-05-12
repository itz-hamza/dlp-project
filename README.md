# 📧 Spam Detection using BiLSTM and BERT

This project demonstrates a deep learning-based approach to email spam classification using two powerful architectures:
- ✅ **Bidirectional LSTM**
- 🤖 **BERT Transformer (Hugging Face)**

The system is designed for email spam classification.

---

## 🚀 Objective

Develop a robust spam classification model that:
- Detects spam emails with high accuracy
- Compares classical deep learning (LSTM) with transformer-based (BERT) architectures

---

## 🧠 Models Used

### 1. Bidirectional LSTM
- Tokenization via `TextVectorization` layer
- Embedding + Bidirectional LSTM
- Dense output with sigmoid activation
- Lightweight and fast to train

### 2. BERT (Transformer)
- `bert-base-uncased` from Hugging Face Transformers
- Preprocessing with `BertTokenizer`
- Fine-tuned using `TFBertForSequenceClassification`
- Better generalization and performance, especially on nuanced data

---

## 📁 Dataset

- Format:
  | text | label |
  |------|-------|
  | "Free money waiting for you!" | 1 |
  | "Meeting rescheduled to 3 PM" | 0 |

- Total Samples: **80,000**
- Split: **80% training / 20% testing**

---
## Results

| Model            | Accuracy | Notes                                |
| ---------------- | -------- | ------------------------------------ |
| BiLSTM           | \~90%    | Lightweight, decent baseline         |
| BERT Transformer | \~94–96% | Best performance, handles complexity |


