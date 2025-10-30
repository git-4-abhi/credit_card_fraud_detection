# credit_card_fraud_detection
Overview
This project detects fraudulent credit card transactions using multiple machine learning models.
The dataset is highly imbalanced, so it’s balanced before training for better performance.

Workflow

Data Loading and Exploration
The dataset creditcard.csv was loaded using pandas.
Checked for missing values (none found).
Observed imbalance: Class 0 represents legitimate transactions, Class 1 represents fraud.

Data Balancing
A random sample of legitimate transactions equal to the number of fraud transactions was selected.
Both subsets were combined to form a balanced dataset.

Splitting Data
Features (X) and target (Y) were separated.
Data was split into training and testing sets using an 80:20 ratio.

Models Used
Logistic Regression
Decision Tree Classifier
Random Forest Classifier
K-Nearest Neighbors (KNN)

Evaluation Metrics
Accuracy Score
Confusion Matrix
Classification Report (Precision, Recall, F1-score)

RESULTS SUMMARY:

Model | Train Accuracy | Test Accuracy | Notes
Logistic Regression | ~93% | ~91% | Baseline model
Decision Tree | ~100% | ~90% | Slight overfitting
Random Forest | ~100% | ~94% | Best performing model
KNN | ~92% | ~88% | Less accurate, simple model

FUTURE IMPROVEMENTS:

This project can be further enhanced in several ways.
First, techniques such as SMOTE or other oversampling methods can be used to improve class balance.
Second, applying normalization or feature scaling can help algorithms like KNN and Logistic Regression perform better.
Third, hyperparameter tuning can be performed to optimize model performance.
Finally, advanced models such as XGBoost or LightGBM can be implemented to achieve higher accuracy and better generalization.
