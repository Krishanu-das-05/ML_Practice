# Random Forest

Practice implementing random forest using bagging (bootstrap aggregation) and majority voting.

**Dataset:** Wine (178 samples, 13 features, 3 classes)

## Results

| Metric | From Scratch | sklearn |
|--------|-------------|---------|
| Accuracy | 0.9722 | 0.9444 |
| Precision | 0.9741 | 0.9463 |
| Recall | 0.9722 | 0.9444 |
| F1 Score | 0.9718 | 0.9440 |

## Key Takeaways

- Random Forest = many decision trees + bootstrap sampling + majority vote
- Bagging reduces overfitting by averaging out individual tree errors
- From-scratch implementation matches/exceeds sklearn on this dataset — confirms correctness of bootstrap + voting logic
- With small n_trees (10), randomness in feature sampling can sometimes hurt rather than help on smaller datasets
- No feature scaling needed for tree-based models — same as single decision trees
