# 🧠 Biomedical Text Fusion Classification

A hybrid biomedical text classification framework that combines **TF-IDF** and **character-level n-gram features** using a **feature fusion approach** to improve contextual and morphological representation. The model is evaluated on the **PubMed 20k RCT dataset**.

---

## 📌 Overview

Biomedical text classification is a critical task in clinical NLP. This project proposes a **multi-feature fusion model** that integrates:

* Contextual information using **TF-IDF**
* Morphological patterns using **character n-grams**
* A **fusion-based representation** for improved classification

The approach demonstrates that combining complementary feature spaces significantly enhances performance.

---

## 🚀 Features

* ✅ TF-IDF based contextual feature extraction
* ✅ Character n-gram feature modeling (3–5 grams)
* ✅ Feature fusion using sparse matrix concatenation
* ✅ Logistic Regression classifier
* ✅ Ablation study (baseline vs proposed model)
* ✅ Evaluation using Accuracy and Macro-F1

---

## 📂 Dataset

This project uses the **PubMed 20k RCT dataset**, which contains labeled sentences from biomedical abstracts.

### Labels:

* BACKGROUND
* OBJECTIVE
* METHODS
* RESULTS
* CONCLUSIONS

---

## 🧠 Methodology

The proposed pipeline consists of three main stages:

1. **Context Representation (TF-IDF)**
   Extracts important terms representing semantic context.

2. **Morphological Feature Extraction (Character N-grams)**
   Captures sub-word patterns and lexical variations.

3. **Feature Fusion and Classification**
   Combines both feature sets and applies a classifier.

---

## ⚙️ Installation

```bash
pip install numpy pandas scikit-learn scipy kagglehub
```

---

## ▶️ Usage

### 1. Download dataset

```python
import kagglehub

path = kagglehub.dataset_download("matthewjansen/pubmed-200k-rtc")
```

### 2. Run the notebook

* Open the provided Kaggle notebook
* Execute all cells

---

## 📊 Results

| Model             | Accuracy | Macro-F1 |
| ----------------- | -------- | -------- |
| TF-IDF            | Baseline | Baseline |
| Char N-gram       | Baseline | Baseline |
| Fusion (Proposed) | Improved | Improved |

👉 The fusion model consistently outperforms individual feature models.

---

## 🔬 Ablation Study

The study evaluates:

* TF-IDF only
* Character n-grams only
* Fusion model

**Conclusion:**
Feature fusion provides complementary learning and improves classification accuracy.

---

## 📈 Evaluation Metrics

* Accuracy
* Macro F1-score
* Classification report

---

## 📌 Key Contribution

* Hybrid feature representation for biomedical text
* Demonstration of complementary feature learning
* Lightweight and efficient model suitable for real-world applications

---

## 🔴 Limitations

* Does not use UMLS or ontology-based features
* No deep learning architecture (can be extended)

---

## 🔮 Future Work

* Integration with **scispaCy / UMLS entity linking**
* Transformer-based models (BERT, BioBERT)
* Graph-based biomedical knowledge integration

---



---

