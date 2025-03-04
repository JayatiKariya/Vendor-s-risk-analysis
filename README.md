# Vendor-s-risk-analysis
**📌 Vendor Risk Analysis & Invoice Prediction System**

## **🚀 Project Overview**
This project focuses on analyzing invoice data to predict vendor payment risks. Initially, **time series forecasting** was attempted for **monthly spending trends**, but the data exhibited **white noise**, making predictions infeasible. Instead, a **Vendor Risk Analysis Model** was developed to classify invoices as **Paid or Pending** based on historical patterns.  

### **📂 Datasets Used:**
- `Invoices_Train_Set1.csv` to `Invoices_Train_Set5.csv` – Invoice records.
- `Payments_Train_Set1.csv` to `Payments_Train_Set5.csv` – Payment history.
- `Vendors.csv` – Vendor details.

 **🛠 Tech Stack**
- **Programming Language:** Python, jupyter notebook.
- **Libraries Used:** Pandas, NumPy, Scikit-learn, XGBoost, FastAPI, Matplotlib, Seaborn, Joblib .
- **Deployment:** FastAPI.

---

 **📊 Steps to Run the Project**
Follow these steps to execute the entire project in order:

 **1️⃣ Run EDA (Exploratory Data Analysis)**
📌 **File:** `eda.ipynb`  
✅ Generates a **pandas profiling report** (`analytics.html`) with insights into the dataset.  

2️⃣ Run Anomaly Detection
📌 File: Anomalies_detection.ipynb
✅ Applies Z-score and IQR methods to check for outliers.
✅ Result: No significant anomalies found in the dataset.

3️⃣ Run Monthly Spending Prediction (Time Series)
📌 File: Monthly_spends_prediction_time_series.ipynb
✅ Attempts time series forecasting using ARIMA, Prophet, and LSTMs.
✅ Result: Data is white noise, making prediction infeasible.

4️⃣ Run Vendor Risk Analysis
📌 File: vendors_risk_analysis.ipynb
✅ Feature Engineering: Vendor frequency, average invoice amount, pending ratio, invoice age.
✅ Trained Multiple ML Models: Random Forest (Best), XGBoost, Logistic Regression, SVM, etc.
✅ Saved the Best Model (vendor_risk_model.pkl) for deployment.
