# Credit Card Fraud Detection using Machine Learning

## Project Overview

This project focuses on detecting fraudulent credit card transactions using Machine Learning. Fraud detection is a critical challenge in the financial industry, where identifying fraudulent transactions quickly can help prevent significant financial losses.

The objective of this project is to build a classification model capable of distinguishing between legitimate and fraudulent transactions using historical transaction data.

---

## Dataset Information

Dataset: Credit Card Fraud Detection Dataset

### Dataset Characteristics

- Total Transactions: 284,807
- Features: 31
- Target Variable: Class

### Target Classes

- Class = 0 → Legitimate Transaction
- Class = 1 → Fraudulent Transaction

The dataset is highly imbalanced, with fraudulent transactions representing only a very small percentage of total transactions.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-Learn
- Jupyter Notebook

---

## Machine Learning Model

### Random Forest Classifier

The Random Forest algorithm was selected because:

- It performs well on classification tasks.
- It reduces overfitting compared to a single Decision Tree.
- It handles large datasets efficiently.
- It provides robust predictive performance.

Model Parameters:

```python
RandomForestClassifier(
    n_estimators=200,
    random_state=42,
    class_weight="balanced"
)
```

---

## Project Workflow

### 1. Data Loading
- Import dataset
- Explore dataset structure

### 2. Data Inspection
- Check dataset shape
- View sample records
- Verify missing values

### 3. Data Preparation
- Separate features and target variable
- Create training and testing datasets

### 4. Model Training
- Train Random Forest Classifier
- Learn transaction patterns

### 5. Fraud Prediction
- Predict fraudulent transactions
- Generate prediction probabilities

### 6. Model Evaluation
- Accuracy Score
- Confusion Matrix
- Classification Report
- ROC-AUC Score

---

## Evaluation Metrics

The model was evaluated using multiple classification metrics:

### Accuracy
Measures overall prediction correctness.

### Precision
Measures how many predicted fraud transactions were actually fraudulent.

### Recall
Measures how many actual fraud transactions were successfully detected.

### F1-Score
Balances Precision and Recall.

### Confusion Matrix
Shows correct and incorrect predictions.

### ROC-AUC Score
Measures the model's ability to distinguish between fraudulent and legitimate transactions.

---

## Why Recall Matters

Fraud detection is an imbalanced classification problem.

Missing a fraudulent transaction can result in financial loss.

Therefore, Recall is one of the most important evaluation metrics for this project.

---

## Business Impact

This system can help:

- Detect suspicious transactions
- Reduce financial fraud losses
- Improve transaction security
- Support financial risk management

---

## Future Improvements

- SMOTE for imbalance handling
- XGBoost implementation
- Hyperparameter tuning
- Feature importance visualization
- Real-time fraud detection system
- Streamlit deployment

---

## Author

Naman Sharma

Machine Learning & Data Science Enthusiast
