# Predicting Car Prices Using Structured and Text-Based Features

**Authors:** Ayyub Orujzade, Agnieszka Dogiel, Alain Kalonji

## 1. Project Overview
This project explores predicting car prices using both **structured numerical features** and **text-based features** (dealer names, customer feedback). We evaluate whether NLP techniques like **LDA, Word2Vec, and TF-IDF** improve prediction performance in a regression task.

**Goal:** Assess the contribution of text-processing methods to car price prediction and explore future directions with advanced NLP embeddings.

---

## 2. Dataset
- **Structured features:** Model, transmission, body style, engine type, etc.
- **Text features:** Dealer_Name, Customer_Feedback
- **Target:** Price

**Source:** `data/car_sales.csv`

---

## 3. Methodology
1. **Data Preprocessing:** Handle missing values, encode categorical features, scale numeric data, train-test split.
2. **Modeling:**
   - Baseline: Random Forest on structured features
   - Extended: Random Forest + text features (LDA, Word2Vec, TF-IDF)
3. **Evaluation:** MAE and RMSE metrics
4. **Feature Importance:** Determine how text features contribute to the prediction

---

## 4. Results
| Model | MAE   | RMSE  |
|-------|-------|-------|
| Baseline (Structured only) | 0.3178 | 0.5721 |
| Text Model (LDA, Word2Vec, TF-IDF) | 0.3198 | 0.5756 |

**Observation:** Text features provided minimal improvement. Structured features dominate price prediction. Future work could explore deep learning embeddings (BERT, GPT) or sentiment analysis.

---

## 5. Future Work
- Apply **Named Entity Recognition (NER)** on dealer names
- Use **sentiment scores** from customer feedback
- Experiment with **contextual embeddings (BERT, GPT)** for richer text representation

---

## 6. How to Run
1. Clone the repository
   ```bash
   git clone https://github.com/Eyyub0491/Text-Mining-Project.git
   cd Text-Mining-Project
