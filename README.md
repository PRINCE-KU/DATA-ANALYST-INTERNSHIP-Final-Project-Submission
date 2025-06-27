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


# 📘 Data Analytics & Data Science Interview Q&A

Welcome to a comprehensive guide of **50 top interview questions and answers** in the field of **Data Analytics & Data Science**. This list is perfect for students, job seekers, and professionals preparing for interviews.

---

## 📌 Table of Contents

- [SQL & Databases](#sql--databases)
- [Statistics & Data Cleaning](#statistics--data-cleaning)
- [Data Analysis & Visualization](#data-analysis--visualization)
- [Machine Learning](#machine-learning)
- [Tools & Projects](#tools--projects)
- [Soft Skills & Scenario-Based](#soft-skills--scenario-based)

---

## 💡 SQL & Databases

1. **What are the key differences between INNER JOIN and OUTER JOIN in SQL?**  
   ➤ INNER JOIN returns matching records, OUTER JOIN returns all records from one or both tables regardless of match.

2. **What is the role of a primary key in a relational database?**  
   ➤ It uniquely identifies each row in a table and ensures no duplicates or nulls.

3. **Explain the concept of normalization in databases.**  
   ➤ Normalization organizes data to reduce redundancy and improve data integrity.

4. **What is the difference between a clustered and non-clustered index?**  
   ➤ Clustered index defines the physical order of data. Non-clustered is a separate structure with pointers to data.

5. **What is the purpose of the GROUP BY clause in SQL?**  
   ➤ It groups rows with the same values to perform aggregate functions like COUNT, SUM, etc.

6. **What are lag and lead functions in SQL?**  
   ➤ They access data from previous or next rows without joins—useful in time-based analysis.

7. **How do you optimize a slow SQL query?**  
   ➤ Use indexing, avoid SELECT *, use WHERE filters, analyze execution plans, and limit joins.

---

## 📊 Statistics & Data Cleaning

8. **How do you handle missing data in a dataset?**  
   ➤ Remove, impute with mean/median/mode, use interpolation, or model-based imputation.

9. **What is the difference between variance and standard deviation?**  
   ➤ Variance is the average squared deviation; std. deviation is its square root.

10. **How would you detect outliers in a dataset?**  
   ➤ Using Z-score, IQR, boxplots, or clustering-based anomaly detection.

11. **How do you handle duplicate data entries in a dataset?**  
   ➤ Use `drop_duplicates()` in Pandas or deduplication logic in SQL.

12. **What is multicollinearity and why is it a problem?**  
   ➤ It occurs when features are highly correlated, affecting model accuracy.

13. **What is a hypothesis test and when would you use it?**  
   ➤ It helps test assumptions (e.g. in A/B testing) using p-values.

14. **How do you ensure data accuracy and integrity in a project?**  
   ➤ Validate sources, normalize data, enforce schema checks, and track anomalies.

---

## 📈 Data Analysis & Visualization

15. **What is data wrangling and why is it important?**  
   ➤ It's cleaning and transforming raw data into a usable format for analysis.

16. **What is a pivot table and how have you used it?**  
   ➤ A summarization tool used in Excel/BI to group and analyze data (e.g. attrition by department).

17. **Explain the differences between a bar chart and a histogram.**  
   ➤ Bar chart = categorical data; histogram = frequency distribution of numerical data.

18. **What is a correlation matrix and how do you interpret it?**  
   ➤ A table of correlation coefficients (from -1 to +1) showing variable relationships.

19. **What is the difference between correlation and causation?**  
   ➤ Correlation shows relationship, but causation means one directly affects the other.

20. **What is the purpose of data visualization?**  
   ➤ To communicate insights clearly and drive decisions.

21. **How do you decide which chart to use for a dataset?**  
   ➤ Based on data type: line for trends, bar for categories, scatter for relationships.

22. **What is the difference between a heatmap and a scatter plot?**  
   ➤ Heatmap shows intensity (color-coded matrix), scatter shows numeric value relationships.

---

## 🤖 Machine Learning

23. **Explain the difference between supervised and unsupervised learning.**  
   ➤ Supervised: labeled data, e.g. classification. Unsupervised: no labels, e.g. clustering.

24. **How do you validate a machine learning model?**  
   ➤ Use train-test split, cross-validation, and metrics like precision, recall, F1-score.

25. **How do you deal with imbalanced datasets?**  
   ➤ Use resampling (SMOTE), class weights, or advanced metrics like ROC AUC.

26. **What is the role of feature engineering in data analysis?**  
   ➤ Creating new features to improve model performance using domain knowledge.

27. **What are the steps of a typical data analysis pipeline?**  
   ➤ Data Collection → Cleaning → Exploration → Modeling → Evaluation → Reporting.

---

## 🛠️ Tools & Projects

28. **Describe a data project where you used Python.**  
   ➤ Built an HR Attrition model using Pandas, Seaborn, Sklearn, and SHAP.

29. **What libraries do you use for data analysis in Python?**  
   ➤ Pandas, NumPy, Seaborn, Matplotlib, Scikit-learn, Plotly, SHAP.

30. **Explain the use of Pandas groupby() function.**  
   ➤ It groups data by a column and applies aggregate functions like sum(), mean().

31. **What is ETL vs ELT?**  
   ➤ ETL: Extract → Transform → Load. ELT: Extract → Load → Transform (used in modern cloud DBs).

32. **What is the difference between OLAP and OLTP systems?**  
   ➤ OLAP = analytics, OLTP = transactions (real-time operations).

33. **Describe your experience with Tableau or Power BI.**  
   ➤ Built dashboards to show KPIs, filter by department, visualize attrition patterns.

34. **What are dimensions and measures in Tableau?**  
   ➤ Dimensions = categories (e.g. department), Measures = numeric fields (e.g. salary).

35. **How do you track data quality over time?**  
   ➤ Automated validation reports, null/missing value tracking, schema monitoring.

36. **What are your favorite Python functions for data analysis?**  
   ➤ `groupby()`, `value_counts()`, `apply()`, `merge()`, `pivot_table()`.

37. **What is time series analysis and where have you used it?**  
   ➤ It analyzes trends over time. Used in forecasting attrition and product demand.

---

## 🎯 Soft Skills & Scenario-Based

38. **Describe a situation where you used data to solve a business problem.**  
   ➤ Helped reduce attrition by analyzing HR data and building a predictive model.

39. **How do you handle large datasets efficiently?**  
   ➤ Use chunking, efficient data types, SQL queries, or distributed processing (e.g. PySpark).

40. **How do you explain complex data insights to non-technical stakeholders?**  
   ➤ Use simple visuals, analogies, focus on business impact, avoid jargon.

41. **What is data cleaning and how do you perform it?**  
   ➤ Fix missing data, duplicates, data type issues, and ensure consistency.

42. **What does the term 'data storytelling' mean to you?**  
   ➤ Communicating insights using narrative, visuals, and impact-driven messaging.

43. **What is A/B testing and how is it used in data analysis?**  
   ➤ Comparing two variants to see which performs better statistically.

44. **What are common KPIs used in business analysis?**  
   ➤ Customer Churn Rate, Net Profit Margin, CAC, Attrition Rate, Conversion Rate.

45. **What is the difference between a data analyst and data scientist?**  
   ➤ Analyst = descriptive analytics; Scientist = predictive modeling and ML.

46. **Describe a challenging dataset you worked on.**  
   ➤ A dataset with mixed types and imbalanced classes. Required SMOTE + feature engineering.

47. **How do you prioritize tasks on multiple data projects?**  
   ➤ Based on deadlines, stakeholder urgency, and business impact.

48. **What steps do you take before starting a data analysis project?**  
   ➤ Define goals, understand stakeholders, assess data quality, and clarify scope.

49. **Describe a time your analysis had a measurable business impact.**  
   ➤ Helped reduce attrition by 12% by identifying risk factors and making data-backed HR recommendations.

50. **How would you analyze user behavior on a website?**  
   ➤ Use page views, session duration, bounce rate, clickstream, and conversion funnel analysis.

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

