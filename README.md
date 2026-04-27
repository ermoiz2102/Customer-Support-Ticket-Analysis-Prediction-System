# 📊 Customer Support Ticket Analysis & Prediction System

## 🚀 Project Overview

This project is an end-to-end **Data Analytics + Machine Learning solution** built on a Customer Support Tickets dataset (2020–2021).

The goal is to:

* Analyze customer support operations
* Identify bottlenecks in ticket resolution
* Generate actionable business insights
* Build a machine learning model to predict whether a ticket will be resolved

---

## 📂 Dataset Information

* Total Records: **8,469 tickets**
* Time Period: **2020–2021**

### Key Features:

* Ticket Details: type, subject, priority, status
* Customer Info: age, gender, satisfaction rating
* Time Data: response time, resolution time
* Product & Channel Information

---

## 🧹 Data Preprocessing

The dataset was cleaned and prepared using:

* Column standardization (lowercase, underscores)
* Datetime conversion for time-based features
* Handling missing values
* Feature engineering:

  * `Status_Group` (Closed vs In Progress)
  * `product_category`
  * `age_group`
  * Encoded categorical variables

---

## 📊 Exploratory Data Analysis (EDA)

Key areas explored:

* Monthly ticket trends
* Ticket priority vs closure rate
* Product category distribution
* Channel usage (Email, Phone, Chat, Social Media)
* Customer demographics
* Satisfaction ratings

---

## 📈 Dashboard

A Power BI dashboard was created to visualize key KPIs:

<img width="1263" height="797" alt="image" src="https://github.com/user-attachments/assets/168d44b0-abb1-4b98-a052-ef1f1bab8c45" />


### Key Metrics:

* Total Tickets: **8,469**
* Avg Response Time: **19.35 hrs**
* Avg Resolution Time: **9.61 hrs**
* Avg Satisfaction Rating: **2.99 / 5**
* Resolved Tickets %: **33%**

---

## 🔍 Key Insights

* ⚠️ **65–69% tickets remain unresolved** → major backlog issue
* ⏱️ **First response time (19 hrs)** is the biggest bottleneck
* 📱 Electronics category generates highest ticket volume
* 📊 All channels handle ~25% traffic → balanced system
* 👥 Customers aged **47–59** generate the most tickets
* ⭐ Customer satisfaction is moderate (**2.99/5**)

---

## 🤖 Machine Learning

### 🎯 Objective

Predict whether a ticket will be:

* **Closed (1)**
* **In Progress (0)**

---

### ⚠️ Avoiding Data Leakage

The following features were removed:

* `resolution_time_hours`
* `customer_satisfaction_rating`

These variables are only available after ticket resolution and would lead to unrealistic model performance.

---

### 🧠 Model Used

* Random Forest Classifier

---

### 📊 Features Used

* Customer demographics (age, gender)
* Ticket type & priority
* Channel (Email, Phone, etc.)
* Product category
* Month of ticket

---



## 🛠 Tech Stack

* **Python** (Pandas, NumPy)
* **Visualization**: Matplotlib, Seaborn
* **Machine Learning**: Scikit-learn
* **Dashboard**: Power BI
* **EDA Report**: Jupyter Notebook

---

## 📁 Project Structure

```
Customer-Support-Analysis/
│
├── data/
│   └── dataset.csv
│
├── notebooks/
│   └── eda_analysis.ipynb
│
├── dashboard/
│   └── dashboard.png
│
├── README.md
```

---

## 💡 Business Impact

This project helps organizations:

* Reduce ticket backlog
* Improve SLA performance
* Prioritize high-risk tickets
* Enhance customer satisfaction

---

## 🚀 Future Improvements

* Deploy model using **Streamlit**
* Add **real-time prediction system**
* Use advanced models (XGBoost, LightGBM)
* Integrate with live customer support systems

---

## 👨‍💻 Author

Moiz Khan
Aspiring Data Scientist | Machine Learning Enthusiast

---
