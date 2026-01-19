# Car Insurance Claim Prediction System

## 📌 Project Overview
This project builds an end-to-end machine learning system to support insurance risk assessment by predicting:

1. Whether a policyholder will file a car insurance claim (classification)
2. The estimated cost of the claim if a claim occurs (regression)

The solution combines data preprocessing, exploratory data analysis, machine learning model development, evaluation, and deployment readiness following industry best practices.

---

## 🎯 Business Objective
Insurance companies face challenges in identifying high-risk customers and estimating potential claim liabilities.  
This project helps insurers to:

- Proactively identify customers likely to file claims
- Estimate expected claim costs for better financial planning
- Improve underwriting and risk-based premium pricing
- Optimize claim management and resource allocation

---

## 🛠️ Tech Stack
- **Programming Language:** Python  
- **Libraries:** Pandas, NumPy, Scikit-learn  
- **Visualization:** Matplotlib, Seaborn  
- **Models:** Logistic Regression, Random Forest, XGBoost, CatBoost, Linear Regression  
- **Deployment:** FastAPI, Docker  

---

## 📊 Dataset Description
- ~8,000 car insurance policyholder records
- Features include:
  - Demographics (age, gender, driving experience)
  - Financial information (annual income)
  - Vehicle details (vehicle age, type)
  - Policy attributes (coverage type)
  - Historical claim information

---

## 🔧 Data Preprocessing & Feature Engineering
The dataset was cleaned and prepared using the following steps:

- Handling missing values using appropriate imputation strategies
- Encoding categorical variables using OneHotEncoding and OrdinalEncoding
- Feature scaling for models sensitive to magnitude
- Outlier treatment for skewed features such as annual income and claim amount
- Feature analysis to identify important risk indicators

This ensured high-quality input data and reduced noise for modeling.

---

## 📈 Exploratory Data Analysis (EDA)
EDA was performed to understand data distributions and feature relationships:

- Correlation heatmaps to identify influential variables
- Boxplots and histograms to detect skewness and outliers
- Countplots to analyze class imbalance and policy distributions

EDA insights guided feature selection and model choice.

---

## 🤖 Modeling Strategy

### Classification – Claim Prediction
Models trained:
- Logistic Regression (baseline)
- Random Forest
- XGBoost
- CatBoost

Evaluation metrics:
- Accuracy
- Precision, Recall, F1-score
- ROC-AUC
- Confusion Matrix

---

### Regression – Claim Cost Prediction
Models trained (only for customers with claims):
- Linear Regression (baseline)
- Decision Tree Regressor
- Random Forest Regressor

Evaluation metrics:
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

---

## 📊 Model Performance

### Classification Results
- Accuracy: ~88%
- ROC-AUC: ~0.91
- Balanced F1-score across classes

### Regression Results
- MAE: ~950
- RMSE: ~1200
- R² Score: ~0.78

These results demonstrate strong predictive capability and generalization.

---

## 🚀 Deployment
The trained models are designed to be deployment-ready:
- Served using **FastAPI** as REST APIs
- Containerized using **Docker** for portability and reproducibility

---

## 📌 Key Takeaways
- Built a complete ML pipeline from raw data to deployment
- Implemented both classification and regression workflows
- Applied best practices to prevent data leakage
- Delivered a business-relevant and scalable solution

---

## ▶️ How to Run the Project
```bash
pip install -r requirements.txt
python app.py
