# Logistic Regression

Practice implementing logistic regression with sigmoid function and binary cross-entropy.

**Dataset:** Breast Cancer Wisconsin (569 samples, 30 features)

## Results

| Metric | From Scratch | sklearn |
|--------|-------------|---------|
| Accuracy | 0.9825 | 0.9737 |
| Precision | 0.9859 | 0.9722 |
| Recall | 0.9859 | 0.9859 |
| F1 Score | 0.9859 | 0.9790 |

## Key Takeaways

- From-scratch implementation slightly outperforms sklearn (98.25% vs 97.37% accuracy) — likely due to sklearn's default L2 regularization
- Sigmoid function maps linear output to [0, 1] probability range for binary classification
- Only 2 misclassifications on the test set (1 false positive, 1 false negative)
- Feature scaling is critical — 30 features with vastly different scales need normalization for gradient descent
