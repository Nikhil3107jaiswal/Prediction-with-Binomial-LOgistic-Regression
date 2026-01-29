# 📊 Bank Marketing Prediction using Logistic Regression

## 🔍 Project Overview
This project focuses on building a **predictive classification model** to determine whether a bank client will **subscribe to a term deposit** based on demographic information, financial attributes, and marketing campaign data.

The model is developed using **Logistic Regression**, following the complete **Machine Learning Life Cycle**, including **EDA, preprocessing, model training, validation, and inference**.

---

## 🎯 Business Objective
To help banks:
- Identify customers with a higher likelihood of subscribing to a term deposit
- Optimize marketing campaigns
- Improve conversion rates and reduce operational costs

---

## 🧠 Problem Statement
Predict the output variable:

**`y` → Has the client subscribed to a term deposit?**  
- `yes` → 1  
- `no` → 0  

This is a **Binary Classification Problem**.

---

## 📁 Dataset Information
- **Dataset**: Bank Marketing Dataset  
- **Rows**: 45,000+  
- **Columns**: 17  
- **Missing Values**: None  

---

## 🧾 Attribute Information

### 🔹 Input Variables
**Bank Client Data**
- `age` – Age of the client  
- `job` – Type of job  
- `marital` – Marital status  
- `education` – Education level  
- `default` – Credit in default (yes/no)  
- `balance` – Average yearly balance  

**Loan Details**
- `housing` – Housing loan (yes/no)  
- `loan` – Personal loan (yes/no)  

**Campaign Details**
- `contact` – Communication type  
- `day` – Last contact day  
- `month` – Last contact month  
- `duration` – Call duration (seconds)  
- `campaign` – Number of contacts during this campaign  
- `pdays` – Days since last contact  
- `previous` – Number of previous contacts  
- `poutcome` – Outcome of previous campaign  

### 🔹 Output Variable
- `y` – Term deposit subscription (`yes` / `no`)

---

## 🔄 Machine Learning Life Cycle Followed
1. Business Understanding  
2. Data Understanding  
3. Exploratory Data Analysis (EDA)  
4. Data Preprocessing  
5. Model Building (Logistic Regression)  
6. Model Evaluation & Validation  
7. Inference & Business Insights  

---

## 📊 Exploratory Data Analysis (EDA)
EDA was performed in a **separate notebook** and included:

- Target variable distribution analysis  
- Age distribution and job-based analysis  
- Balance vs subscription behavior  
- Loan status vs subscription  
- Call duration impact analysis  
- Categorical feature analysis using count plots  
- Numerical feature analysis using boxplots and histograms  

### 🔍 Key EDA Insights
- Dataset is **imbalanced** (more `no` than `yes`)
- Clients with **higher balances** are more likely to subscribe
- **Longer call durations** significantly increase subscription probability
- Retired and student segments show higher conversion
- Clients without housing or personal loans subscribe more

---

## 🧹 Data Preprocessing
- Converted target variable (`y`) into binary format
- One-Hot Encoding applied to categorical variables
- Feature scaling performed using **StandardScaler**
- Stratified train-test split to handle class imbalance

---

## 🤖 Model Building
- Algorithm Used: **Logistic Regression**
- Reason:  
  - Suitable for binary classification  
  - Interpretable coefficients  
  - Efficient and robust  

---

## 📈 Model Evaluation Metrics
- Accuracy Score  
- Precision  
- Recall  
- F1-Score  
- ROC-AUC Score  
- Confusion Matrix  
- ROC Curve  

### 🧪 Model Performance
- The model demonstrates **good predictive capability**
- ROC-AUC score confirms strong class separation
- Performs significantly better than random guessing

---

## 🧠 Feature Importance (Inference)
Top influential factors affecting subscription:
1. Call duration  
2. Previous campaign outcome  
3. Account balance  
4. Age  
5. Campaign interaction history  

---

## 📌 Final Business Insights
✔ Longer customer interaction increases subscription probability  
✔ High-balance customers are more responsive  
✔ Previous campaign success is a strong predictor  
✔ Loan-free clients have higher conversion rates  

---

## 💡 Business Recommendations
- Focus marketing efforts on high-value customers
- Improve call engagement quality and duration
- Re-target customers with previous successful interactions
- Optimize campaign frequency to avoid customer fatigue

---

## 🛠️ Tools & Technologies Used
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Scikit-learn**
- **Jupyter Notebook**

---

## 📂 Project Structure
