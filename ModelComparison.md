# Model Comparison — Heart Disease Prediction

**Dataset:** 241 training samples, 61 test samples, 30 features

---

## Test Set Metrics

| Model | Accuracy | Precision | Recall | F1-score | AUC-ROC |
|-------|----------|-----------|--------|----------|---------|
| Logistic Regression | 0.8361 | 0.8485 | 0.8485 | 0.8485 | 0.9048 |
| Decision Tree | 0.7213 | 0.7500 | 0.7273 | 0.7385 | 0.7992 |
| Random Forest | 0.8197 | 0.8235 | 0.8485 | 0.8358 | 0.8820 |
| KNN | 0.8361 | 0.8485 | 0.8485 | 0.8485 | 0.9053 |

---

## Accuracy Comparison

```
KNN                  ████████████████████████████████████████░░░░░░░░  83.61%
Logistic Regression  ████████████████████████████████████████░░░░░░░░  83.61%
Random Forest        ██████████████████████████████████████░░░░░░░░░░  81.97%
Decision Tree        ██████████████████████████████████░░░░░░░░░░░░░░  72.13%
```

## AUC-ROC Comparison

```
KNN                  ███████████████████████████████████████████████░  90.53%
Logistic Regression  ██████████████████████████████████████████████░░  90.48%
Random Forest        ████████████████████████████████████████████░░░░  88.20%
Decision Tree        ████████████████████████████████████████░░░░░░░░  79.92%
```

## F1-score Comparison

```
KNN                  ████████████████████████████████████████░░░░░░░░  84.85%
Logistic Regression  ████████████████████████████████████████░░░░░░░░  84.85%
Random Forest        ████████████████████████████████████████░░░░░░░░  83.58%
Decision Tree        ███████████████████████████████████░░░░░░░░░░░░░  73.85%
```

---

## Best Model by Each Metric

| Metric | Best Model | Score |
|--------|-----------|-------|
| Accuracy | KNN / Logistic Regression | 0.8361 |
| Precision | KNN / Logistic Regression | 0.8485 |
| Recall | KNN / Logistic Regression / Random Forest | 0.8485 |
| F1-score | KNN / Logistic Regression | 0.8485 |
| AUC-ROC | KNN | 0.9053 |

---

## Ranking

| Rank | Model | Accuracy | F1-score | AUC-ROC |
|------|-------|----------|----------|---------|
| 1 | KNN | 0.8361 | 0.8485 | 0.9053 |
| 2 | Logistic Regression | 0.8361 | 0.8485 | 0.9048 |
| 3 | Random Forest | 0.8197 | 0.8358 | 0.8820 |
| 4 | Decision Tree | 0.7213 | 0.7385 | 0.7992 |

---

## Key Findings

- **KNN** and **Logistic Regression** are virtually tied as the best performers, with identical accuracy (83.61%) and F1-scores (0.8485). KNN has a marginally higher AUC-ROC (0.9053 vs 0.9048).

- **Random Forest** comes in third with solid performance across all metrics (81.97% accuracy, 0.882 AUC-ROC).

- **Decision Tree** has the lowest performance (72.13% accuracy), which is expected as it is a simpler model prone to overfitting on small datasets.
