# Credit-Card-Fraud-Detection
Predict fraudulent transactions and visualize financial risk using Python, scikit-learn, and Power BI


# Project Overview

Fraudulent credit card transactions are a major financial risk for banks and payment processors.
This project builds an end-to-end fraud detection system to identify suspicious transactions and provide business-ready risk insights.

*Objective:* Detect fraudulent credit card transactions and provide business-ready insights using Python (Pandas, scikit-learn, imbalanced-learn), and deliver a Power BI dashboard 

# Key highlights:

Analyzed 284,807 transactions and detected 492 fraud cases (0.17%).

Built ML models to classify fraud vs legitimate transactions.

Designed a Power BI dashboard for fraud trend monitoring and KPI reporting.

# Workflow

## 1. Data Cleaning & EDA

Handled missing values, duplicates, and outliers.

Feature engineering: Transaction_Hour, Amount_bin.

Visualized fraud distribution by time and amount.

<img width="721" height="393" alt="image" src="https://github.com/user-attachments/assets/5764bc5b-0705-48a7-8b0b-595f28d06324" />





<img width="844" height="410" alt="image" src="https://github.com/user-attachments/assets/79cde5d4-e35b-4839-b6b7-5a5a19af7173" />









## 2. Feature Scaling & Imbalance Handling

Used StandardScaler for numeric normalization.

Balanced data using SMOTE to address extreme class imbalance.


## 3. Model Training & Evaluation

Compared Logistic Regression and Random Forest.

*Technical Interpretation*

ROC-AUC = 0.982 --> Overall model discrimination ability (1 = perfect) and model can distinguish fraud vs legit 98.2% of the time.

Precision (for fraud = 1) = 0.54 --> % of predicted frauds that were actually fraud and of every 100 flagged transactions, 54 are real frauds.

Recall (for fraud = 1) = 0.85 --> % of actual frauds that were correctly detected and model catches 85% of all fraud cases — high detection rate.

F1-Score = 0.66 --> Balance between Precision & Recall and solid balance; acceptable trade-off in fraud use cases.

Accuracy (weighted) ≈ 100% --> Overall correct predictions and looks perfect because of heavy imbalance (99.8% legit). Not a reliable metric here.


<img width="524" height="455" alt="image" src="https://github.com/user-attachments/assets/9e73d540-0472-46d1-a9a8-1504310bc092" />





<img width="831" height="547" alt="image" src="https://github.com/user-attachments/assets/62807842-9feb-46ff-8cbb-0f1fb15944cb" />



## 4. Conclusion 

Random Forest model is highly accurate, with strong recall and excellent AUC, which is exactly what fraud teams prioritize — catching as many frauds as possible, even if some false alarms occur. We are going to choose Logistic Regression with its 97% accuracy, with its ROC-AUC Score of 0.9713.

<img width="846" height="547" alt="image" src="https://github.com/user-attachments/assets/a2405262-53bd-43ac-b5fc-e96be877f175" />



# Business Impact

✅ Enables early detection of potential fraud losses before transaction settlement.

✅ Provides actionable insights for fraud team prioritization.

✅ The system can catch 85 out of 100 fraud cases, allowing early prevention of financial losses with manageable false alerts.


*Metric focus:* In highly imbalanced fraud tasks, prioritize Recall (catch frauds) at acceptable Precision and monitor Precision (top K risky transactions). Use PR-AUC to measure the model's ability to find fraud.


# Dashboard



<img width="854" height="482" alt="image" src="https://github.com/user-attachments/assets/2bdb6449-f260-494d-9fe9-9fba06924645" />








# Author

Gourav Sarkar

🎓 M.A. Economics | Data Analyst | Python, SQL, Power BI, Machine Learning
