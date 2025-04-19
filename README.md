# 🚗 Car Price Prediction - Regression Modeling Project

## 📌 Project Overview

A Chinese automobile company plans to enter the US market and wants to understand how car prices are determined in the American context. This project uses various regression algorithms to model and predict car prices based on a wide range of features such as engine size, weight, mileage, horsepower, and more.

The key objectives are:
- Identify significant variables affecting car prices
- Understand the strength of their impact
- Build predictive models for pricing strategy optimization

---

## 📁 Dataset

- **Source**: Provided CSV file (`CarPrice_Assignment.csv`)
- **Content**: Contains information about 205 different car models with features like:
  - `enginesize`, `horsepower`, `curbweight`, `carwidth`, etc.
  - Car name and brand
  - Fuel type, drive wheels, body style, etc.
  - **Target Variable**: `price`

---

## ✅ Project Structure & Steps

### 1. 🔄 Loading and Preprocessing
- Cleaned and structured the data
- Extracted brand names from car names
- Fixed spelling inconsistencies
- Encoded categorical variables using One-Hot Encoding
- Scaled numerical features using `StandardScaler`
- Split the dataset into training and testing sets (70/30)

### 2. 🤖 Model Implementation
Implemented the following five regression algorithms:
- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor
- Support Vector Regressor (SVR)

### 3. 📊 Model Evaluation
Evaluated models based on:
- **R² Score**
- **Mean Squared Error (MSE)**
- **Mean Absolute Error (MAE)**

📈 **Best Model**: Random Forest Regressor  
🏆 R² Score: 0.92 (before tuning), improved to 0.94 (after tuning)

### 4. 🔍 Feature Importance Analysis
Identified the most influential features using Random Forest:
- `enginesize`, `curbweight`, `highwaympg`, `horsepower`, `carwidth`
- Engine size alone contributed over **54%** to model performance

### 5. 🛠️ Hyperparameter Tuning
Used `GridSearchCV` to optimize Random Forest parameters:
- Tuned `n_estimators`, `max_depth`, `min_samples_split`, `min_samples_leaf`
- Improved performance in all metrics

---

## 📈 Final Results Summary

| Model                | R² Score | MSE         | MAE     |
|---------------------|----------|-------------|---------|
| Random Forest (Tuned)| **0.94** | 891243.20   | 693.81  |
| Gradient Boosting    | 0.89     | 1270041.22  | 812.56  |
| Decision Tree        | 0.85     | 1654011.00  | 965.32  |
| Linear Regression    | 0.83     | 1867234.89  | 1035.61 |
| Support Vector Regr. | 0.71     | 2501293.12  | 1178.87 |

---

## 📂 Technologies Used

- Python 3.10+
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`
- Jupyter Notebook for implementation

---

## 📌 Conclusion

This project successfully:
- Identified key features influencing car prices
- Built accurate models to predict car prices
- Enabled data-driven decisions for entry into the US automobile market

---

## 🧠 Author
**Your Name**  
[GitHub Profile](https://github.com/yourusername)  
**Date**: April 2025

---

## ✅ How to Run
1. Clone the repository
2. Open `Car_Price_Prediction.ipynb` in Jupyter Notebook
3. Run all cells to see data preprocessing, modeling, and evaluation in action

---

