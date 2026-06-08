# Linear Regression

Practice implementing linear regression from scratch using gradient descent.

**Dataset:** California Housing (20,640 samples, 8 features)

## Results

| Metric | From Scratch | sklearn |
|--------|-------------|---------|
| MSE | 0.5559 | 0.5559 |
| RMSE | 0.7456 | 0.7456 |
| R2 Score | 0.5758 | 0.5758 |

## Key Takeaways

- From-scratch implementation matches sklearn perfectly when gradient descent converges
- Learning rate is critical — too low = slow convergence, too high = divergence
- Feature scaling (StandardScaler) is essential for gradient descent to work properly
- R2 of 0.58 means linear regression explains 58% of variance — dataset has non-linear relationships that a linear model can't capture
