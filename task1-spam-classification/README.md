# Spam Email Classification (Task 1)

This project builds a machine learning model to classify messages as **spam** or **ham (normal)**.

---

## Method

Three approaches were compared:

### 1. TF-IDF + Logistic Regression
Traditional text representation capturing keyword importance.

### 2. Sentence-BERT Embeddings
Dense semantic embeddings generated using a pretrained transformer model.

### 3. Combined Features
TF-IDF vectors concatenated with Sentence-BERT embeddings.

---

## Training

Hyperparameters were tuned using **GridSearchCV** with **5-fold cross-validation**, optimizing the **F1 score**.

---

## Evaluation Metrics

Models were evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC

---

## Results

| Model | Accuracy | F1 Score |
|------|------|------|
| TF-IDF | 0.9848 | 0.9849 |
| SBERT | 0.9793 | 0.9794 |
| Combined | **0.9890** | **0.9890** |

The combined feature representation achieved the best performance.

---

## Files

spam_classification.ipynb  
Main notebook containing the experiment.

spam_results.csv  
Evaluation results generated from the experiments.