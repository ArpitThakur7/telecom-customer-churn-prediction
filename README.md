# 📞 Telecom Customer Churn Prediction

## 📌 Overview
This project aims to predict customer churn in a telecom company using machine learning models.

Customer churn refers to customers leaving a service. By identifying patterns and factors that lead to churn, companies can take proactive steps to retain customers and improve business performance.

---

## 📊 Dataset
- Source: IBM Telco Customer Churn Dataset
- Records: ~7000 customers
- Features: 21 variables including:
  - Demographics (gender, senior citizen)
  - Account information (tenure, contract)
  - Services (internet, streaming, security)
  - Billing (monthly & total charges)
  - Target variable: **Churn (Yes/No)** :contentReference[oaicite:0]{index=0}

---

## ⚙️ Technologies Used
- Python 🐍
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn

---

## 🔍 Data Preprocessing
- Removed unnecessary column (`customerID`)
- Handled missing values in `TotalCharges`
- Converted categorical variables using **Label Encoding**
- Removed outliers using IQR method
- Applied feature scaling (StandardScaler)

---

## 📈 Exploratory Data Analysis (EDA)

### Key Insights:

- Only **~26.49% customers churned** :contentReference[oaicite:1]{index=1}  
- Customers with **low tenure (<5 months)** have higher churn  
- **Month-to-month contracts** show higher churn  
- Customers with **higher monthly charges** are more likely to churn  
- Customers using **streaming services churn less**

---

## 🤖 Models Used

1. Decision Tree Classifier  
2. Random Forest Classifier  
3. K-Nearest Neighbors (KNN)  

---

## ⚙️ Model Training
- Train-test split applied
- Hyperparameter tuning using GridSearchCV

---

## 📊 Model Performance

| Model              | Accuracy |
|-------------------|---------|
| Decision Tree      | ~79%    |
| Random Forest      | ~82% ✅ |
| KNN                | ~79%    |

👉 Random Forest performed best with highest accuracy and F1-score :contentReference[oaicite:2]{index=2}  

---

## 📉 Evaluation Metrics
- Accuracy Score  
- F1 Score  
- Mean Squared Error  
- Mean Absolute Error  
- Confusion Matrix  

---

## 🔑 Feature Importance

Top important features:
- Tenure  
- Contract Type  
- Monthly Charges  
- Total Charges :contentReference[oaicite:3]{index=3}  

---

## 📌 Conclusion

- Customer retention strongly depends on tenure and contract type  
- High monthly charges increase churn probability  
- Random Forest is the most effective model for this dataset  

This model can help telecom companies:
- Predict customer churn  
- Improve retention strategies  
- Optimize pricing and services  

---

## 🚀 How to Run

1. Clone repository
```bash
git clone https://github.com/yourusername/telecom-customer-churn-prediction.git
