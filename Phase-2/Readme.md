Phase 2: Model Training & Evaluation


Overview
In this phase, machine learning models are applied to the preprocessed dataset to predict fraudulent transactions (is_fraud). The goal is to compare multiple algorithms and evaluate their performance using appropriate metrics.

Models Implemented

1. Logistic Regression
A statistical model used for binary classification
Predicts probability of fraud (0 or 1)
Works well for linearly separable data

3. K-Nearest Neighbors (KNN)
Instance-based learning algorithm
Classifies data based on nearest neighbors
Sensitive to feature scaling

5. Support Vector Machine (SVM)
Finds optimal boundary (hyperplane) between classes
Effective in high-dimensional spaces
Works well with scaled data

Evaluation Metrics Used
Accuracy
Measures overall correctness of the model
Formula:
Accuracy = (TP + TN) / Total
Precision
Measures correctness of positive predictions (fraud detection)
Important when false positives matter
Formula:

Precision = TP / (TP + FP)
Confusion Matrix
Provides detailed breakdown of predictions:

Predicted 0
Predicted 1
Actual 0
TN
FP
Actual 1
FN
TP
Helps understand:
False positives (normal marked as fraud)
False negatives (fraud missed)
ROC Curve (Receiver Operating Characteristic)
Plots:
True Positive Rate (TPR)
vs False Positive Rate (FPR)
Used to evaluate model performance at different thresholds
Workflow
Split dataset into training and testing sets
Train models:
Logistic Regression
KNN
SVM
Make predictions on test data
Evaluate using:
Accuracy
Precision
Confusion Matrix
ROC Curve & AUC Score
Outcome
Comparison of models based on performance metrics
Identification of best-performing model for fraud detection
Understanding trade-offs between accuracy and precision
