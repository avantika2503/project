Dataset:  IMDB dataset having 50K movie reviews for natural language processing or Text analytics.
https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews/data
Accuracy: 94.2% using DistilBERT model
# Sentiment Analysis of IMDb Movie Reviews using DistilBERT

This repository contains the implementation for my research work **“Sentiment Analysis of Movie Reviews Using Deep Learning and NLP Models,”** published at **IEEE ICPCT 2025**.

The project evaluates classical NLP techniques (Bag-of-Words, TF–IDF, GloVe) and contrasts them with a fine-tuned **DistilBERT transformer model**, achieving a highest accuracy of **94.15%**, outperforming multiple state-of-the-art baselines.

---

## 📌 Overview

The goal of the project is to classify IMDb movie reviews as *positive* or *negative* by experimenting with:

- Traditional ML models  
- Feature extraction techniques  
- Deep learning models  
- Transformative pretrained architectures (DistilBERT)

A detailed comparison of accuracy, precision, recall, F1-score, and training behaviour is included, consistent with the methodology in the published paper.

---

## 📁 Repository Structure

📦 Sentiment-Analysis-IMDb
├── BERT FINAL.ipynb # Fine-tuned DistilBERT implementation
├── bag-of-words.ipynb # Bag-of-Words + ML classifiers
├── tfidf (1).ipynb # TF-IDF + ML classifiers
└── README.md # Project documentation



---

## 📊 Dataset

We used the **IMDb 50K Movie Reviews Dataset**, which consists of:

- 25,000 positive reviews  
- 25,000 negative reviews  
- English text only  
- Balanced labels  

Dataset link:  
https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews/data

---

## 🔧 Techniques Implemented

### **Lexicon-based Methods:**
- Bag-of-Words  
- TF-IDF  
- GloVe embeddings  

Trained using classifiers such as:
- Logistic Regression  
- SVM  
- SGD  
- Random Forest  
- XGBoost  
- Multinomial Naive Bayes  
- KNN  
- Decision Tree  

Tables for accuracy comparison available in the paper:
- Table 1 (Bag-of-Words) — page 4  
- Table 2 (TF–IDF) — page 5  
:contentReference[oaicite:2]{index=2}

---

### **Deep Learning Method: DistilBERT**

DistilBERT is a compressed version of BERT, retaining 95% of its performance while being faster and lighter.

Training details (from *Section III-E*, page 3):

- Tokenization with attention masks  
- 80:20 train-test split  
- Trained for **3 epochs**  
- Observed accuracy progression:  
  - Epoch 1: 93.5%  
  - Epoch 2: 94.1%  
  - Epoch 3: **94.15%**
---

## 🏆 Final Results

### **Highest accuracy achieved (our research):**
### 🎯 **94.15% using DistilBERT**  

### Comparison with literature:

| Model | Accuracy |
|--------|----------|
| **DistilBERT (Ours)** | **94.15%** |
| RoBERTa (2023) | 86.31% |
| BERT (2023) | 90.67% |
| Naive Bayes (2020) | 92% |
| CNN-LSTM Hybrid (2019) | 89.2% |
| Passive Aggressive Classifier (2023) | 90.27% |
| USE (2022) | 84.49% |
| Logistic Regression (2022) | 88% |

(Shown in *Table 3* and *Fig. 6*.)  
:contentReference[oaicite:5]{index=5}

---

## 📈 Evaluation Metrics Used

From *Section III-F* (page 4):  
:contentReference[oaicite:6]{index=6}

- Accuracy  
- Precision  
- Recall  
- F1-score  
- Loss curves  
- Confusion matrix  

These metrics were compared across all feature extraction + classifier combinations.

---

## 🔍 Sample Inference

You can test a custom review using the last cell of `BERT FINAL.ipynb`.

Example:
Review: "This movie was beautifully directed and emotionally rich."
Output: Positive (0.97)


---

## 📚 Publication

This project was published at the:

### **IEEE International Conference on Recent Advances in Computational Techniques (ICPCT 2025)**  
DOI: https://doi.org/10.1109/ICPCT64145.2025.10940336

---

## 🧠 Key Takeaways

- DistilBERT captures semantic context far better than classical ML.  
- Lexicon-based models plateau below ~88% accuracy.  
- Transformers scale exceptionally on large textual datasets.  
- Methodology from preprocessing → feature extraction → classifier comparison is essential.  
- Model performance is **heavily influenced** by tokenization quality.  

---

## 👩‍💻 Author

**Avantika Yadav**  
B.Tech CSE — Manipal University Jaipur  
Email: avantiika.yadav@gmail.com  

