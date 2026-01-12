# Credit Card Default Risk Assessment 🏦📊

## 📌 Project Overview
Banks face significant financial risk from customers defaulting on credit card payments.  
This project analyzes **customer demographic and financial behavior data** to **predict the likelihood of credit card default**, helping financial institutions make informed risk management decisions.

The project focuses on **exploratory data analysis (EDA)** and **machine learning modeling** to assess default risk on **July credit card statements**.

---

## 🎯 Business Objective
The goal of this project is to:
- Identify **key factors contributing to credit card default**
- Analyze **customer repayment behavior patterns**
- Build **predictive models** to assess default risk
- Support **data-driven credit and risk management decisions**

---

## 📂 Dataset Description
The dataset contains customer-level information related to demographics, credit usage, billing statements, and repayment history.

### Key Feature Groups
- **Demographics**
  - Age
  - Sex
  - Education Level
  - Marital Status

- **Financial Information**
  - Credit Limit
  - Monthly Statement Amounts (Jan–Jun)
  - Previous Payment Amounts (Jan–Feb)

- **Repayment Behavior**
  - Monthly repayment status from January to June

### 🎯 Target Variable
- **July_Payment_Status**
  - `0` → Paid on time  
  - `1` → Defaulted  

---

## 🛠 Project Workflow

### 1️⃣ Data Understanding & Exploration
- Dataset shape and structure analysis
- Summary statistics and data types
- Distribution analysis of the target variable
- Initial insights into default frequency

---

### 2️⃣ Data Cleaning & Preprocessing
- Removed:
  - Invalid target labels
  - Duplicate records
  - Rows with missing values
- Normalized categorical variables:
  - Sex
  - Education
  - Marital Status
- Addressed skewed numerical features using:
  - Box plots
  - Log transformations

---

### 3️⃣ Exploratory Data Analysis (EDA)
Key analytical questions explored:
- How does **repayment history** affect default risk?
- Do **credit limits** influence default behavior?
- Are there demographic patterns in default rates?
- Does **delinquency duration** increase default probability?

#### Key Insights
- Repayment status is the **strongest indicator of default**
- Customers delayed by more than **2 months** show high default probability
- Financial behavior outweighs demographic influence

---

### 4️⃣ Feature Engineering
- Segregated numerical and categorical features
- Applied log transformation to reduce skewness
- Performed **train-test split with stratification** to maintain class balance

---

## 🤖 Machine Learning Models

### Models Implemented
- **Logistic Regression**
  - Interpretable baseline model
- **Random Forest Classifier**
  - Captures non-linear relationships and feature interactions

### Evaluation Metrics
- Confusion Matrix
- ROC–AUC Curve
- Classification Accuracy
- Recall and Precision

---

## 📈 Model Performance Summary

| Model | Observations |
|------|-------------|
| Logistic Regression | Strong baseline with high interpretability |
| Random Forest | Improved performance and better default detection |

The **Random Forest model** demonstrated superior performance in identifying high-risk customers.

---

## 🔍 Key Findings
- Repayment behavior is the most influential predictor
- Longer delinquency periods significantly increase default risk
- Credit limit and age show moderate impact
- Machine learning enhances traditional credit risk assessment

---

## 🧰 Tech Stack
- **Python**
- **Pandas & NumPy** – Data manipulation
- **Matplotlib & Seaborn** – Data visualization
- **Scikit-learn** – Machine learning
- **Jupyter Notebook** – Analysis and experimentation

