# Anomaly Detection with Isolation Forest
This kernel will use and evaluate the Isolation Forest anomaly detection model to detect fraudulent transactions. The dataset, attained from Kaggle, has its features scaled, and the names of those features are not shown due to privacy concerns.
## Objectives
1. Understand the distribution of the data that was provided
2. Implement the Isolation Forest algorithm
3. Evaluate the model using a train/test split
4. Visualize the results using a confusion matrix
## Background
Fraud detection is a unique machine learning problem. As fradulent transactions can range from <1% to ~10% of all transacations, the resulting dataset will be unbalanced. There will be significantly more "Normal" or legitimate transactions than there will be "Abnormal" or fraudulent ones. Using these datasets to train our machine learning models will introduce a strong bias toward the normal observations, as if it classifies all transactions as normal the model will register a 90+ accuracy rate. This however is not the outcome that we would like to achieve. 
## Model Selection
Isolation Forest is an anomaly detection technique that uses the assumption that anomalies are unique and infrequent. This means that if we were to try to isolate the point by randomly choosing partitions across various features, on average, these anomalies would require fewer trees to be isolated.
We will use the credit card dataset to test this algorithm and evaluate the performance of the model given this dataset.
