# Fraud Detection

## Project Overview

This project is part of my **Data Analytics Internship — Level 2, Task 3**.

The objective is to develop a machine learning model capable of detecting fraudulent credit card transactions using historical transaction data. The project focuses on exploratory data analysis, handling class imbalance, feature engineering, model training and performance evaluation.

Two machine learning algorithms, **Logistic Regression and Random Forest**, are implemented and compared to identify an effective fraud detection approach.

## Dataset

- **Source:** Kaggle
- **Dataset:** Credit Card Transactions Fraud Detection
- **Dataset Link:** https://www.kaggle.com/datasets/kartik2112/fraud-detection
- **File Used:** `fraudTrain.csv`
- **Target Variable:** `is_fraud`

The dataset contains simulated financial transactions with information such as transaction amount, transaction time, merchant category, customer characteristics and fraud labels.

## Technologies Used

- Python
- pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- KaggleHub
- Jupyter Notebook / Google Colab

## Project Workflow

### 1. Data Collection and Cleaning

- Loaded the dataset directly from Kaggle using KaggleHub.
- Inspected dataset dimensions, data types and missing values.
- Converted transaction timestamps into datetime format.
- Prepared numerical and categorical variables for modeling.

### 2. Exploratory Data Analysis

- Analysed fraudulent and legitimate transaction counts.
- Calculated the percentage of fraudulent transactions.
- Compared transaction amounts across classes.
- Investigated fraudulent transactions by hour of day.
- Analysed fraud rates across merchant categories.

### 3. Feature Engineering

Created additional features, including:

- Transaction hour and day of week
- Customer age
- Customer-to-merchant geographical distance
- Log-transformed transaction amount

### 4. Handling Class Imbalance

Fraudulent transactions represent a small proportion of the dataset.

Class-weight balancing was used to give greater importance to minority-class errors during model training.

### 5. Model Development

Trained and compared:

1. Logistic Regression
2. Random Forest Classifier

The dataset was divided into training and testing sets using an 80/20 stratified split.

### 6. Model Evaluation

Models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Precision–Recall analysis
- Confusion Matrix

### 7. Feature Importance

Random Forest feature importance and Logistic Regression coefficients were analysed to understand the variables associated with fraud predictions.

## Visualizations

- Fraud vs Legitimate Transactions
- Transaction Amount Distribution
- Fraud Rate by Hour
- Fraud Rate by Merchant Category
- Confusion Matrices
- ROC Curves
- Precision–Recall Curves
- Feature Importance Charts

## Results

The project generates a comparison of Logistic Regression and Random Forest using classification metrics.

**Add your actual results after executing the notebook:**

| Model | Precision | Recall | F1-score | ROC-AUC |
|---|---|---|---|---|
| Logistic Regression | TBD | TBD | TBD | TBD |
| Random Forest | TBD | TBD | TBD | TBD |

The final model can be selected based on the trade-off between detecting fraudulent transactions and minimizing false-positive alerts.

## How to Run

1. Clone or download this repository.
2. Install the required Python libraries.

```bash
pip install kagglehub pandas numpy matplotlib seaborn scikit-learn
```

3. Open the Jupyter Notebook.
4. Run the cells in sequence.
5. The dataset will be downloaded through KaggleHub.

## Output Files

- `fraud_model_comparison.csv`
- `fraud_feature_importance.csv`

## Conclusion

This project demonstrates the application of data analytics and machine learning to fraudulent transaction detection. It highlights the importance of class imbalance handling, appropriate evaluation metrics and identifying transaction patterns that may indicate fraud.

## Future Improvements

- Hyperparameter tuning
- Cross-validation
- Cost-sensitive threshold optimisation
- Real-time fraud prediction API
- Model drift monitoring

## Author

**K Shivaram Goud**  
Data Analytics Intern  
B.Tech — Artificial Intelligence and Machine Learning