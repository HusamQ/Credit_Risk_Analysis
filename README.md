# Credit_Risk_Analysis

# Summary and Analysis of Results
To apply machine learning to solve a real-world challenge: credit card risk
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, I employ different techniques to train and evaluate models with unbalanced classes. The random forest classifier, with and without AdaBoost, failed to achieve useable performance. The balanced random forest classifier's precision is 0.04, meaning that in 100 loan applications that were flagged to be bad, only 4 were actually bad loan applications. The model's recall/sensitivity is 0.67, meaning that it detected 67% of bad loan applications. The F1 score is low at 0.07, since either a low precision or recall will result in a lower F1 score.

# Credit_Risk resampling Technique summary: 

The random forest classifier with AdaBoost, while achieving better results, still suffered from inadequate predictive power. Its precision score is 0.09 and its recall 0.92. The F1 score, again, is skewed low at 0.16 by the low precision score.

The performances of both models are insufficient for commercial application.Summary and Analysis of Results
Oversampling, both naive and with SMOTE, did not yield a useable model for the prediction of bad loans. Naive oversampling resulted in a precision score of 0.01 and recall of 0.62. The F1 score of 0.02 reflected athe low precision score. SMOTE oversampling similarly resulted in a precision score of 0.01 and recall of 0.61, and a F1 score of 0.02.

A model with undersampling yielded similarly poor results, with a precision score of 0.01, recall of 0.65, and F1 score of 0.01.

Combination sampling resulted in a precision score of 0.01 and recall of 0.70, and a F1 score of 0.02. While the recall score is marginally better than that of the other models, the overall performance of the model is still poor.

These models are inadequately predictive, and are not recommended for commercial application.
