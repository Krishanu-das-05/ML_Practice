# Gradient Boosting

Practice implementing gradient boosting with sequential weak learners that correct previous errors.

**Dataset:** Breast Cancer Wisconsin (569 samples, 30 features, binary)

## Results

| Metric | sklearn |
|--------|---------|
| Accuracy | 0.9561 |
| Precision | 0.9583 |
| Recall | 0.9718 |
| F1 Score | 0.9650 |

### Learning Rate Experiment

| Learning Rate | Accuracy |
|---------------|----------|
| 0.001 | 0.6228 |
| 0.01 | 0.9561 |
| 0.1 | 0.9561 |
| 0.5 | 0.9649 |
| 1.0 | 0.9649 |
| 2.0 | 0.9737 |

## Key Takeaways

- Gradient Boosting builds trees sequentially, each correcting previous errors via residuals
- Learning rate and n_estimators trade off — too low a learning rate with fixed estimators causes underfitting (62% at lr=0.001)
- Unlike raw gradient descent, boosting frameworks have built-in stability (shrinkage) making them less prone to divergence
- From-scratch Logistic Regression (98.25%) outperformed Gradient Boosting (95.61%) on this dataset — complexity doesn't always win on simple, well-separated data
- XGBoost/LightGBM are production-optimized versions with regularization, speed, and missing value handling
