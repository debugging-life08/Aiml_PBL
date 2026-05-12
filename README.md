Fraud Detection System using Machine Learning

Project Overview This project focuses on building a fraud detection system using machine learning techniques. The goal is to classify financial transactions as fraudulent (1) or legitimate (0) based on various features such as transaction amount, location, time, and user details.

Dataset Description The dataset contains transaction-level information including:

Transaction details (amt, trans_date_trans_time) User information (city, state, job, dob) Location data (lat, long, merch_lat, merch_long) Target variable: is_fraud

Data Preprocessing Steps The dataset was cleaned and prepared using the following steps:

Data Understanding Checked structure using .info(), .describe() Identified missing values Data Cleaning Dropped unnecessary columns (index, trans_num) Removed duplicate records Handling Missing Values Numerical columns → filled with mean Categorical columns → filled with mode Feature Engineering Extracted: trans_hour, trans_day, trans_month, weekday Converted dob → age Dropped original datetime columns Encoding Categorical Variables One-Hot Encoding: category, state Label Encoding: merchant, city, job Outlier Detection & Treatment Used IQR method Visualized using boxplots Handled outliers in: amt, city_pop, age Geographic features (lat, long) left unchanged Feature Scaling Applied StandardScaler Normalized all feature values for better model performance

Machine Learning Models The following models are implemented: 1.Logistic Regression 2.K-Nearest Neighbors (KNN) 3.Support Vector Machine (SVM)

Workflow Data Collection → Data Cleaning → Feature Engineering → Encoding → Outlier Handling → Scaling → Model Training → Evaluation Evaluation Metrics

Models are evaluated using:

1.Accuracy 
2.Precision 
3.Recall 
4.F1-score 
5.Confusion Matrix
