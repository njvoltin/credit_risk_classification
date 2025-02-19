# Overview of the Analysis

The purpose of this analysis was to build a machine learning model to predict whether a loan is At_Risk (1) or Healthy (0) based on financial data. The dataset contained various financial attributes that were used to classify individuals into these two categories.

The target variable in this analysis was loan_status, which had two classes:

    Healthy (0): Majority class
    At_Risk (1): Minority class

The data was processed through the following machine learning pipeline:

    Data Preprocessing – Handling missing values, encoding categorical variables, and standardizing numerical features.

    Feature Selection – Identifying the most relevant financial features contributing to classification.

    Model Selection and Training – Using LogisticRegression to train a binary classification model.

    Evaluation – Measuring the model’s performance using accuracy, precision, recall, and F1-score.

A Logistic Regression model was chosen due to its interpretability and effectiveness in binary classification tasks.

Results

Machine Learning Model: Logistic Regression

    Accuracy: 99%
    Precision (Healthy - 0): 1.00
    Recall (Healthy - 0): 1.00
    Precision (At_Risk - 1): 0.87
    Recall (At_Risk - 1): 0.95
    F1-score (At_Risk - 1): 0.91

Summary

The Logistic Regression model performed exceptionally well, achieving an overall accuracy of 99%. The model demonstrated perfect classification for the majority class (Healthy - 0), with both precision and recall at 1.00. However, for the minority class (At_Risk - 1), precision was slightly lower (0.87), meaning some Healthy loans were misclassified as At_Risk. The recall for the At_Risk category was 0.95, meaning the model correctly identified most individuals who were truly at risk.

Recommendation

The model performs best at correctly identifying Healthy loans (0) with perfect accuracy.

If the goal is to minimize false negatives (i.e., avoid missing an At_Risk loan), this model is effective because it has a high recall (0.95) for At_Risk cases.

However, if reducing false positives (wrongly classifying Healthy loans as At_Risk) is more important, the model might require adjustments such as tuning the decision threshold or balancing the dataset using another tool.

Overall, the Logistic Regression model is a strong choice for this classification problem, but further adjustments could be made depending on the business needs and tolerance for misclassification errors.

