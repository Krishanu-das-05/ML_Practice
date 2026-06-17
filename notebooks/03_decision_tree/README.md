# Decision Tree

Practice implementing a decision tree classifier using Gini impurity for splitting.

**Dataset:** Iris (150 samples, 4 features, 3 classes)

## Results

| Metric | From Scratch | sklearn |
|--------|-------------|---------|
| Accuracy | 1.0000 | 1.0000 |
| Precision | 1.0000 | 1.0000 |
| Recall | 1.0000 | 1.0000 |
| F1 Score | 1.0000 | 1.0000 |

## Key Takeaways

- Decision trees handle multiclass classification naturally — no modification needed unlike logistic regression
- No feature scaling required — decision trees split on threshold values, not distances
- Iris is a well-separated dataset — perfect accuracy is expected and achievable
- From-scratch implementation matches sklearn exactly, confirming correct Gini-based splitting logic
- max_depth controls overfitting — deeper trees memorize training data
- For multiclass evaluation metrics, use average='weighted' to account for class sizes
