# 🚚 E-Commerce Delivery Intelligence & Customer Experience Analytics

### End-to-End Business Analytics & Machine Learning Project on 100,000 Quick-Commerce Orders

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green)
![Scikit-Learn](https://img.shields.io/badge/Machine%20Learning-ScikitLearn-orange)
![XGBoost](https://img.shields.io/badge/XGBoost-Gradient%20Boosting-red)
![Status](https://img.shields.io/badge/Project-Completed-success)

---

# 📌 Project Overview

This project analyzes **100,000 e-commerce delivery transactions** across India's leading quick-commerce platforms:

* JioMart
* Blinkit
* Swiggy Instamart

The objective is to transform raw delivery data into actionable business insights using data analytics, statistics, customer segmentation, sentiment analysis, and machine learning.

The project follows a complete analytics workflow from raw data preprocessing to predictive modeling and business recommendations.

---

# 🎯 Business Problem

Quick-commerce companies face several operational and customer experience challenges:

* Delivery delays impact customer satisfaction
* Refund requests increase operational costs
* Customer feedback is difficult to analyze at scale
* Businesses struggle to identify valuable customers
* Decision-makers require data-driven insights for operational improvement

This project addresses these challenges through analytical and predictive techniques.

---

# 📊 Dataset Information

### Dataset Summary

| Metric             | Value   |
| ------------------ | ------- |
| Records            | 100,000 |
| Features           | 11      |
| Missing Values     | 0       |
| Duplicate Records  | 0       |
| Platforms          | 3       |
| Product Categories | 6       |

### Features Included

| Feature           | Description          |
| ----------------- | -------------------- |
| Platform          | Delivery Platform    |
| Order Value       | Revenue per Order    |
| Delivery Time     | Delivery Duration    |
| Service Rating    | Customer Rating      |
| Delivery Delay    | Delay Indicator      |
| Refund Requested  | Refund Status        |
| Customer Feedback | Review Text          |
| Product Category  | Product Type         |
| Order Hour        | Order Placement Time |
| Customer ID       | Customer Identifier  |
| Order Date        | Transaction Date     |

---

# 🏗️ Project Workflow

```text
Raw Dataset
     │
     ▼
Data Cleaning
     │
     ▼
Feature Engineering
     │
     ▼
Exploratory Data Analysis
     │
     ▼
Business Insights
     │
     ├── Statistical Testing
     ├── RFM Analysis
     └── Sentiment Analysis
     │
     ▼
Machine Learning Models
     │
     ├── Refund Prediction
     └── Rating Prediction
     │
     ▼
Business Recommendations
```

---

# 📂 Repository Structure

```bash
Ecommerce-Delivery-Analytics/

│
├── data/
│   ├── Ecommerce_Delivery_Analytics_New.csv
│   ├── cleaned_data.csv
│   ├── cleaned_with_sentiment.csv
│   └── rfm_segments.csv
│
├── notebooks/
│   ├── 01_Data_Cleaning.ipynb
│   ├── 02_EDA.ipynb
│   ├── 03_Business_Insights.ipynb
│   ├── 04_RFM_Analysis.ipynb
│   ├── 05_Sentiment_Analysis.ipynb
│   ├── 06_Refund_Prediction.ipynb
│   └── 07_Rating_Prediction.ipynb
│
├── visuals/
│   └── Project Visualizations
│
├── requirements.txt
│
└── README.md
```

---

# 🔍 Exploratory Data Analysis

The EDA phase focused on understanding delivery operations and customer behavior.

### Analysis Performed

* Platform-wise delivery performance
* Delivery time distribution
* Refund rate analysis
* Service rating distribution
* Revenue analysis by category
* Peak-hour order analysis
* Delay frequency analysis

### Key Deliverables

✔ KPI Scorecards

✔ Comparative Platform Analysis

✔ Revenue Insights

✔ Customer Experience Trends

✔ Operational Performance Metrics

---

# 📈 Business Insights & Statistical Analysis

Two major business hypotheses were evaluated.

## Hypothesis 1

### Does Delivery Delay Impact Customer Ratings?

**Test Used:** Independent Sample T-Test

**Result:** Not Statistically Significant

**p-value > 0.05**

---

## Hypothesis 2

### Do Delivery Delays Increase Refund Requests?

**Test Used:** Chi-Square Test

**Result:** Not Statistically Significant

**p-value > 0.05**

---

### Key Observation

The dataset demonstrates minimal correlation between operational variables and customer outcomes.

Rather than forcing business conclusions, the analysis accurately reports findings supported by statistical evidence.

This demonstrates practical application of analytical methodology and statistical decision-making.

---

# 👥 Customer Segmentation (RFM Analysis)

Customers were segmented using the RFM Framework.

### Recency

How recently a customer placed an order.

### Frequency

How often the customer places orders.

### Monetary Value

Total customer spending.

### Segments Generated

* Champions
* Loyal Customers
* Potential Loyalists
* New Customers
* Need Attention
* At Risk
* Hibernating
* Lost Customers

### Business Applications

* Retention Campaigns
* Loyalty Programs
* Personalized Marketing
* Customer Re-engagement Strategies

---

# 😊 Sentiment Analysis

Customer reviews were transformed into measurable sentiment indicators.

### Sentiment Categories

* Positive
* Neutral
* Negative

### Themes Identified

* Delivery Speed
* Product Quality
* Packaging
* Order Accuracy
* Delivery Experience

### Outcome

Converted qualitative customer feedback into actionable business intelligence.

---

# 🤖 Machine Learning Models

## 1️⃣ Refund Prediction Model

### Business Objective

Predict whether a customer is likely to request a refund based on operational and order-related features.

### Algorithms Evaluated

* Logistic Regression
* Random Forest Classifier
* XGBoost Classifier

### Features Used

* Platform
* Delivery Time
* Order Value
* Product Category
* Delivery Delay
* Order Hour
* Engineered Features

### Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1-Score
* ROC-AUC Score
* Confusion Matrix

### Model Evaluation Summary

| Model               | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
| ------------------- | -------- | --------- | ------ | -------- | ------- |
| Logistic Regression | 0.4924   |  0.4516   | 0.5029 | 0.4759   | 0.4925  |
| Random Forest       | 0.5076   | 0.4648    | 0.4929 | 0.4784   | 0.5031  |
| XGBoost             | 0.5379   | 0.4519    | 0.0399 | 0.0734   | 0.4994  |

### Key Observation

The classification models performed close to random guessing, indicating a lack of predictive signal between operational features and refund behavior.

This finding was validated through:

* Correlation Analysis
* Statistical Testing
* Feature Importance Analysis

### Business Interpretation

The dataset does not provide strong evidence that delivery time, platform, order value, or category significantly influence refund requests.

The project demonstrates proper machine learning methodology rather than forcing artificial predictive performance.

---

## 2️⃣ Customer Rating Prediction Model

### Business Objective

Predict customer service ratings using operational and transaction-related features.

### Algorithms Evaluated

* Ridge Regression
* Random Forest Regressor
* XGBoost Regressor

### Features Used

* Platform
* Delivery Time
* Order Value
* Product Category
* Delivery Delay
* Order Hour
* Engineered Features

### Evaluation Metrics

* R² Score
* RMSE (Root Mean Squared Error)
* MAE (Mean Absolute Error)
* MSE (Mean Squared Error)

### Model Evaluation Summary

| Model                   | R² Score | RMSE                 | MAE                  |
| ----------------------- | -------- | -------------------- | -------------------- | 
| Ridge                   | -0.0001  | 1.5803               | 1.4841               | 
| Random Forest Regressor | -0.0029  | 1.5824               | 1.4850               | 
| XGBoost Regressor       | -0.0034  | 1.5828               | 1.4850               | 

### Key Observation

All regression models produced R² values near zero, suggesting that available features explain almost none of the variation in customer ratings.

### Business Interpretation

Customer ratings appear largely independent of operational variables in this dataset.

The results support the conclusion that customer ratings were likely generated independently from delivery performance indicators.

---

## 🏆 Model Selection & Comparison

### Classification Task (Refund Prediction)

| Metric Considered |
| ----------------- |
| Accuracy          |
| Precision         |
| Recall            |
| F1-Score          |
| ROC-AUC           |

### Regression Task (Rating Prediction)

| Metric Considered |
| ----------------- |
| R² Score          |
| RMSE              |
| MAE               |

### Final Conclusion

Although predictive performance was limited due to the dataset's synthetic nature, the project successfully demonstrates:

✔ Data Preprocessing

✔ Feature Engineering

✔ Train-Test Splitting

✔ Model Training

✔ Hyperparameter Evaluation

✔ Classification Metrics

✔ Regression Metrics

✔ Model Comparison

✔ Statistical Validation

✔ Business Interpretation of Results


---

# 🛠️ Tech Stack

## Programming Language

* Python

## Data Analysis

* Pandas
* NumPy

## Data Visualization

* Matplotlib
* Seaborn

## Statistics

* SciPy
* Statsmodels

## Machine Learning

* Scikit-Learn
* XGBoost

## Development Environment

* Jupyter Notebook

---

# 🚀 Installation & Execution

Clone the repository:

```bash
git clone https://github.com/saniyacarvalho21/Ecommerce-Delivery-Analytics.git
```

Move to project folder:

```bash
cd Ecommerce-Delivery-Analytics
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Run notebooks sequentially from:

```text
01_Data_Cleaning.ipynb
↓
02_EDA.ipynb
↓
03_Business_Insights.ipynb
↓
04_RFM_Analysis.ipynb
↓
05_Sentiment_Analysis.ipynb
↓
06_Refund_Prediction.ipynb
↓
07_Rating_Prediction.ipynb
```

---

# 📌 Future Enhancements

* Interactive Streamlit Dashboard
* Power BI Business Dashboard
* Real-World E-Commerce Dataset Integration
* Delivery Time Forecasting
* Customer Churn Prediction
* Recommendation System
* Cloud Deployment
* MLOps Integration

---

# 💼 Skills Demonstrated

* Data Cleaning & Preprocessing
* Exploratory Data Analysis (EDA)
* Feature Engineering
* Statistical Hypothesis Testing
* Customer Segmentation
* Sentiment Analysis
* Machine Learning
* Predictive Analytics
* Business Intelligence
* Data Visualization
* Analytical Storytelling

---

# 👩‍💻 Author

## Saniya Carvalho

**Data Analyst | Business Analyst | Machine Learning Enthusiast**

### Connect With Me

LinkedIn:
https://www.linkedin.com/in/saniya-carvalho/

GitHub:
https://github.com/saniyacarvalho21

---

# ⭐ Support

If you found this project useful, consider giving it a star on GitHub.

---

# 📈 Project Tagline

### Turning E-Commerce Delivery Data into Actionable Business Intelligence.
