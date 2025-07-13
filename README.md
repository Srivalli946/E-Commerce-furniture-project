# E-Commerce-furniture-project
# 🪑 E-commerce Furniture Sales Prediction

This project explores an e-commerce dataset of furniture items scraped from AliExpress to understand market trends and build predictive models that estimate the number of units sold based on product features.

---

## 📊 Project Overview

- **Domain**: E-commerce / Retail Analytics  
- **Tools Used**: Python, Pandas, Scikit-learn, Seaborn, Matplotlib  
- **Level**: Beginner  
- **Goal**: Predict product sales volume using product attributes like price, title, and shipping information.

---

## 🧠 Problem Statement

Can we build a machine learning model that accurately predicts how many units of a furniture product will be sold online, based on features such as:

- Product title (textual data)
- Price
- Shipping tags (categorical data)

---

## 📁 Dataset Description

The dataset contains **2,000** entries and the following features:

| Column         | Description                                       |
|----------------|---------------------------------------------------|
| `productTitle` | Name of the furniture product                     |
| `originalPrice`| Price before discount (often missing)             |
| `price`        | Final listed price                                |
| `sold`         | Number of items sold                              |
| `tagText`      | Shipping information (e.g., "Free shipping")      |

---

## 🚀 Workflow Summary

### 1. Data Preprocessing
- Dropped rows with missing values
- Cleaned and converted `price` column
- Encoded `tagText` using Label Encoding
- Removed `originalPrice` due to high missing values

### 2. Exploratory Data Analysis (EDA)
- Visualized price and sold distributions
- Investigated relationship between price and units sold

### 3. Feature Engineering
- Applied **TF-IDF** vectorization to `productTitle` (text feature)
- Merged text features with numerical data

### 4. Model Building
- Trained two regression models:
  - Linear Regression
  - Random Forest Regressor

### 5. Evaluation Metrics
- **Mean Squared Error (MSE)**
- **R² Score**

---

## 📈 Model Performance (Sample Output)

| Model              | MSE (↓)     | R² Score (↑) |
|-------------------|--------------|--------------|
| Linear Regression |  25923.96    |   0.02       |
| Random Forest     |  7498.35     |   0.72       |

> ✅ **Random Forest** typically performs better due to its ability to capture non-linear patterns.

---

 
[🔗 LinkedIn](http://linkedin.com/in/srivalli-uppalapati)

---

## 💡 Future Improvements

- Feature Importance Analysis  
- Hyperparameter Tuning  
- Model Deployment with Streamlit or Flask  
- Time-Series Forecasting (if date info is available)  

---

## 🛡️ Disclaimer

This project is intended for educational and portfolio purposes only. The dataset was ethically sourced and processed in compliance with AliExpress platform standards.

