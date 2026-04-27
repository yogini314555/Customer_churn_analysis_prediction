# Customer_churn_analysis_prediction

📌 Project Overview

This project focuses on analyzing customer churn behavior and building a machine learning model to predict whether a customer will leave a telecom service.

It combines:

📊 Data Analysis (EDA)
🧠 Machine Learning (Random Forest)
📈 Power BI Dashboard
🌐 Flask Web Application
🎯 Objective
Identify key factors driving customer churn
Analyze customer behavior & patterns
Build a predictive model (~85% accuracy)
Deploy a real-time churn prediction system
Help businesses reduce churn & increase retention
📊 Dashboard Preview
🔹 Churn Analysis Summary
6 ![Churn Dashboard]("C:\Users\HP\Downloads\data_analyst_project-20260424T094122Z-3-001\data_analyst_project\customer_churn\summary_churn.png")
🔹 Churn Prediction Dashboard
8
🗂️ Project Structure
📁 Customer-Churn-Analysis
│
├── 📊 Power BI Dashboard
│   └── churn analysis.pbix
│
├── 📓 Notebooks
│   ├── Churn Analysis - EDA.ipynb
│   ├── Churn Analysis - Model Building.ipynb
│   └── Analysis.ipynb
│
├── 🤖 Model
│   ├── model.sav
│   └── best_churn_pipeline.pkl
│
├── 🌐 Flask App
│   ├── app.py
│   └── templates/
│
├── 📄 Dataset
│   └── first_telc.csv
│
└── 📘 Documentation
    └── Project_Report.docx
🧠 Machine Learning Model
Algorithm Used: Random Forest Classifier
Accuracy: ~85%
Features Used:
Demographics (Gender, SeniorCitizen)
Services (Internet, Security, Support)
Billing (MonthlyCharges, PaymentMethod)
Tenure
🔥 Prediction Logic (Flask)

The model:

Takes 19 input features
Applies same preprocessing (encoding + tenure grouping)
Predicts:
✅ Churn / Not Churn
📊 Probability Score

📄 Backend logic available here:
👉

📊 Key Insights
📉 Month-to-Month contracts → Highest churn
💰 High Monthly Charges → High churn risk
🛡️ No Tech Support / Security → More churn
👴 Senior citizens → Higher churn
💳 Electronic check users → High churn
⏳ Tenure < 12 months → Highest churn
📈 Power BI Dashboard Features
KPI Cards:
Total Customers
Total Churn
Churn Rate
Churn Analysis by:
Gender
Age Group
Contract Type
Payment Method
Services
Heatmaps & Segmentation
Interactive Filters

📄 Full dashboard guide:
👉

🛠️ Tech Stack
Tool	Purpose
Python	Data Analysis & ML
Pandas	Data Processing
Scikit-learn	Model Building
Power BI	Dashboard
SQL	Data Analysis
Flask	Web App Deployment
⚙️ Installation & Setup
1️⃣ Clone Repository
git clone https://github.com/your-username/customer-churn-analysis.git
cd customer-churn-analysis
2️⃣ Install Dependencies
pip install -r requirements.txt
3️⃣ Run Flask App
python app.py
4️⃣ Open in Browser
http://127.0.0.1:5000/
🧪 How It Works
User enters customer details
Data is preprocessed (same as training)
Model predicts churn
Output shown with confidence score
📊 SQL Analysis

This project includes:

100+ SQL queries
Advanced analytics
Window functions
Business insights queries

Examples:

-- Churn Rate
SELECT 
    COUNT(CASE WHEN churn='Yes' THEN 1 END)*100.0 / COUNT(*) AS churn_rate
FROM customer_churn;

-- High Risk Customers
SELECT *
FROM customer_churn
WHERE tenure < 12 AND MonthlyCharges > 80;
📌 Business Impact
Identify high-risk customers early
Improve customer retention strategies
Reduce revenue loss
Enable data-driven decisions
🚀 Future Improvements
🔮 XGBoost / LightGBM models
📊 SHAP Explainability
🌐 React Frontend
☁️ Cloud Deployment (AWS / Azure)
🔁 Automated ML Pipeline
🗣️ Interview Explanation

“This project analyzes customer churn using EDA and machine learning. I built a Random Forest model with ~85% accuracy and deployed it using Flask. The system predicts churn based on customer behavior and helps businesses reduce churn by identifying high-risk users.”

👩‍💻 Author

Yogini Virkar
📊 Data Analyst | 💻 SQL | 📈 Power BI | 🤖 Machine Learning
