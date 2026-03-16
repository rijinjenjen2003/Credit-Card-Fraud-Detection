# Credit Card Fraud Detection using Machine Learning

## Project Overview
Credit card fraud is a major problem in the financial industry. Detecting fraudulent transactions is challenging because fraud cases are extremely rare compared to normal transactions.

This project builds a Machine Learning model to detect fraudulent credit card transactions using a real-world dataset.

The main challenge in this dataset is class imbalance, where fraudulent transactions represent a very small percentage of the total data.

---

## Dataset

Dataset Source: Kaggle Credit Card Fraud Detection Dataset

Dataset Information:
- Total Transactions: 284,807
- Fraud Transactions: 492
- Normal Transactions: 284,315
- Features: 31 columns

Feature Description:
- Time – Time elapsed between transactions
- Amount – Transaction amount
- V1–V28 – PCA-transformed anonymized features
- Class – Target variable  
  - 0 → Normal Transaction  
  - 1 → Fraud Transaction

The features V1–V28 were transformed using Principal Component Analysis (PCA) to protect sensitive customer information.

---

## Project Workflow

### 1. Data Loading
Loaded the dataset using Pandas.

### 2. Exploratory Data Analysis (EDA)
Performed data analysis to understand:
- Class distribution
- Feature correlations
- Fraud patterns

### 3. Handling Imbalanced Data
The dataset is highly imbalanced. To solve this problem, SMOTE (Synthetic Minority Over-sampling Technique) was used to balance the dataset.

### 4. Train-Test Split
The dataset was split into training and testing sets.

### 5. Model Training
The following Machine Learning models were used:

- Logistic Regression
- Random Forest Classifier

### 6. Model Evaluation
Models were evaluated using:

- Precision
- Recall
- F1 Score
- Confusion Matrix
- ROC-AUC Score

Accuracy alone is not suitable for imbalanced datasets, so recall and F1-score were considered important metrics.

### 7. Model Selection
Random Forest performed better in detecting fraudulent transactions compared to Logistic Regression.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn (SMOTE)

---

## Visualizations

The project includes visualizations such as:

- Class Distribution Plot
- Correlation Heatmap
- Confusion Matrix
- ROC Curve

---

## Future Improvements

Possible improvements include:

- Hyperparameter tuning
- Testing additional algorithms such as XGBoost
- Building a real-time fraud detection API
- Deploying the model using Flask or FastAPI

---

## Author

Rijin Jenjen  
B.Tech in Electronics and Communication Engineering  
Aspiring Data Scientist
