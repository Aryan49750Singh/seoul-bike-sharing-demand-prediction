# 🚴‍♂️ Seoul Bike Sharing Demand Prediction

## 📌 Problem Statement

Urban bike-sharing systems require efficient demand prediction to ensure availability and minimize waiting time.
This project focuses on predicting the **number of rental bikes required per hour** in Seoul based on environmental and temporal factors.

---

## 📊 Dataset Description

The dataset includes historical bike rental data along with weather and time-based features.

### 🔑 Features:

* **Date** – Year-Month-Day
* **Hour** – Hour of the day
* **Rented Bike Count** – Target variable
* **Temperature (°C)**
* **Humidity (%)**
* **Windspeed (m/s)**
* **Visibility (10m)**
* **Dew Point Temperature (°C)**
* **Solar Radiation (MJ/m²)**
* **Rainfall (mm)**
* **Snowfall (cm)**
* **Seasons** – Winter, Spring, Summer, Autumn
* **Holiday** – Yes/No
* **Functional Day** – Functional / Non-functional

---

## 🔍 Exploratory Data Analysis (EDA)

* Analyzed seasonal trends in bike demand
* Observed peak demand during working hours
* Identified strong correlation with **temperature and hour**
* Detected impact of **rainfall and snowfall** on demand

---

## ⚙️ Feature Engineering

* Converted categorical variables using encoding
* Extracted useful time-based insights from date
* Handled missing/null values
* Scaled numerical features for better model performance

---

## 🤖 Models Implemented

* Linear Regression
* Ridge Regression (with hyperparameter tuning)
* Lasso Regression (with hyperparameter tuning)
* KNN Regressor

---

## 📈 Model Performance

### 🔹 KNN Regressor

* Training Score: **0.8739**
* MAE: **201.91**
* RMSE: **306.77**
* R² Score: **0.7721**
* Adjusted R²: **0.7660**

---

### 🔹 Linear Regression (Best Performing Model)

* Training Score: **0.8345**
* MAE: **199.99**
* RMSE: **289.57**
* R² Score: **0.7969**
* Adjusted R²: **0.6096**

---

### 🔹 Ridge Regression

* Training Score: **0.6476**
* MAE: **294.26**
* RMSE: **385.17**
* R² Score: **0.6407**
* Adjusted R²: **0.6311**

---

## 🏆 Key Insights

* **Linear Regression performed best** with highest R² score
* Weather conditions significantly affect demand
* Peak usage occurs during **commuting hours**
* Extreme weather (rain/snow) reduces bike usage

---

## ▶️ How to Run

1. Clone the repository
2. Open the notebook in Jupyter/Colab
3. Install dependencies:

```
pip install -r requirements.txt
```

4. Run all cells

---

## 🛠 Tech Stack

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn

---

## 🚀 Future Improvements

* Try advanced models (XGBoost, Random Forest)
* Deploy model using Streamlit
* Add real-time prediction system

---

## 📌 Conclusion

This project demonstrates an **end-to-end machine learning pipeline**, including data preprocessing, feature engineering, model training, evaluation, and comparison.

---
