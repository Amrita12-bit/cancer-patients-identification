# cancer-patients-identification
 The project focuses on cancer patient identification using a dataset of over 15,000 records. Various machine learning models including regression, Random Forest, and XGBoost are applied to classify patients. A comparative study evaluates accuracy, precision, recall, and F1-score to determine the best-performing model.
Project Overview

This project focuses on the identification and prediction of cancer patients using a dataset of more than 15,000 records. The main objective is to apply various machine learning models and perform a comparative study to evaluate which model performs best for cancer diagnosis prediction.
 
 Dataset
The dataset contains clinical features for cancer patients.
Each record includes multiple attributes such as tumor size, cell characteristics, and diagnosis labels.
The target column diagnosis is binary:
M = Malignant (cancerous)
B = Benign (non-cancerous)

 Methodology

Data Preprocessing
Dropped irrelevant columns (id, Unnamed: 32).

Encoded diagnosis labels (Malignant → 1, Benign → 0).

Standardized all numerical features using StandardScaler.

Clustering
Applied KMeans Clustering with 3 clusters.
Added cluster labels back into the dataset to strengthen model performance.

Train-Test Split
80% of data used for training, 20% for testing.

Models Implemented
Logistic Regression (baseline regression model)
Random Forest Classifier (tree-based ensemble model)
Neural Network (MLPClassifier) (deep learning approach)

Evaluation Metrics
Accuracy
Precision
Recall
F1-score
Classification reports

 Results
Model	Accuracy
Logistic Regression	~Good baseline
Random Forest	Higher accuracy
Neural Network (MLP)	Competitive performance

 The Random Forest and Neural Network models performed better compared to Logistic Regression, with Random Forest giving a balanced trade-off of accuracy, interpretability, and efficiency.

 Conclusion
Random Forest emerged as the best-performing model for this dataset, as it consistently provided high accuracy and robust predictions.

Neural Network also performed strongly, but required more computation and training time.

Logistic Regression, while simpler, was less accurate, but useful as a baseline.
