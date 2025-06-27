# DATA-ANALYST-INTERNSHIP-Final-Project-Submission
# HR Analytics – Predict Employee Attrition 💼📊

## 📌 Objective

Employee attrition is one of the most crucial concerns in Human Resource Management. The aim of this project is to analyze HR data and uncover the key drivers of employee attrition (resignation), and to predict which employees are likely to leave the company. This allows HR teams to intervene early, improve retention strategies, and build a more satisfied, productive workforce.

Through a combination of Exploratory Data Analysis (EDA), machine learning models, and SHAP explainability tools, this project delivers actionable insights and a predictive system that classifies employees at risk of attrition. The insights are further visualized with Power BI to make the findings more interactive and business-friendly.

---

## 🧰 Tools & Technologies

- **Python** – Data preprocessing, visualization, and machine learning
- **Pandas / NumPy** – Data wrangling and manipulation
- **Seaborn / Matplotlib** – Graphical EDA
- **Scikit-learn** – ML algorithms and model evaluation
- **SHAP (SHapley Additive exPlanations)** – Model explainability
- **Power BI** – Dashboard creation and visual storytelling
- **Jupyter Notebook** – Development environment

---

## 📁 Dataset Overview

- Source: IBM HR Analytics dataset
- Format: CSV
- Total Rows: 1,470
- Features: 35 columns including:
  - Demographics: Age, Gender, Marital Status, Education
  - Job Info: Department, Job Role, Job Level, Monthly Income
  - Work-related: Overtime, Environment Satisfaction, YearsAtCompany
  - Label: `Attrition` (Yes/No)

---

## 📊 Exploratory Data Analysis (EDA)

EDA was performed to identify trends and patterns that may be associated with employee resignations. Major findings include:

- **OverTime is a strong indicator**: Employees doing overtime show a higher chance of attrition.
- **JobRole and Department**: Certain job roles (e.g., Sales Executive, Laboratory Technician) show higher attrition.
- **Monthly Income**: Employees with lower income tend to leave more often.
- **Promotion**: Employees with no promotion in recent years are more likely to resign.
- **Years at Company**: Attrition is most common during the 2–5 year period.

All trends were visualized using bar charts, box plots, and distribution graphs with Seaborn.

---

## 🤖 Machine Learning Models

Three classification models were built and evaluated:

### 1. Logistic Regression
- Baseline model
- Quick to train and interpret
- Accuracy: ~83%

### 2. Decision Tree Classifier
- Better interpretability
- Accuracy: ~86%
- Shows non-linear decision boundaries

### 3. Random Forest Classifier
- Ensemble method with better performance
- Accuracy: ~87%
- Robust against overfitting

#### 🔍 Model Evaluation:
- Accuracy Score
- Confusion Matrix
- Classification Report (Precision, Recall, F1-Score)
- ROC Curve and AUC Score

---

## 🧠 SHAP Value Analysis (Model Explainability)

To interpret model decisions and identify feature importance, SHAP was used. The SHAP summary plot and beeswarm visualizations show:

- **OverTime**: Most important feature
- **Job Role**, **MonthlyIncome**, and **YearsAtCompany** are also key factors
- Allows HR to understand “why” a prediction was made for any individual employee

---

## 📈 Power BI Dashboard

An interactive Power BI dashboard was built with the following features:

### 📊 Overview Page
- Total Employees, Attrition Rate (%), Avg Salary, Avg Age
- Attrition by Department and Gender
- Monthly Income Boxplot
![Screenshot (346)](https://github.com/user-attachments/assets/a93679d8-4b67-413d-a167-16f076d5d3bf)




### 📉 Attrition Risk Analysis
- Overtime vs Attrition
- Attrition by Job Role and YearsAtCompany
- Promotion History Impact

### 🔮 Prediction Insights
- Actual vs Predicted Labels
- Top SHAP Features
- Filterable reports by department, gender, or education

---

## 📝 Recommendations & Suggestions

Based on the analysis, here are some actionable suggestions for HR:

- **Review workloads for employees doing overtime**
- **Implement fair and transparent promotion policies**
- **Increase retention efforts during employees' 2–5 year period**
- **Provide mentorship and training to job roles with higher resignation rates**
- **Address compensation concerns for lower-income staff**

---

## 📂 Project Structure

HR_Attrition_Analytics/
│
├── data/
│ └── WA_Fn-UseC_-HR-Employee-Attrition.csv
│
├── notebooks/
│ └── HR_Attrition_Model.ipynb
│
├── output/
│ └── model_predictions.csv
│
├── dashboard/
│ └── HR_Attrition_Dashboard.pbix
│
├── README.md

