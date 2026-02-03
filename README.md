# Black Friday Sales Prediction 🛍️
Predicting purchase amounts using Linear Regression

## 📌 Project Overview
This project analyzes customer purchase behavior during Black Friday sales to predict the purchase amount for various products. By understanding the relationship between customer demographics (Age, Gender, Marital Status, City Category) and their spending habits, businesses can optimize inventory and marketing strategies.

**Goal:** Predict the purchase amount (`Purchase`) for customers based on demographic and product data.

## 🔍 Key Findings & Methodology
We chose **Linear Regression** as our baseline model. While more complex models (like XGBoost) exist, Linear Regression offered specific advantages for this business case:
1.  **Interpretability:** It allows us to quantify exactly how much factors like "City Category" or "Gender" contribute to the final purchase amount in dollars.
2.  **Speed:** Trains in milliseconds on ~550k rows, compared to minutes/hours for ensemble methods.
3.  **Generalization:** Less prone to overfitting on noisy retail data compared to high-variance models.

**Key Insight:** Demographic factors provided a stable baseline for prediction, with specific product categories driving significant variance in spending.

## 🛠️ Tech Stack
* **Python** (Data Analysis & Modeling)
* **Pandas & NumPy** (Data Manipulation)
* **Matplotlib & Seaborn** (Visualization)
* **Scikit-Learn** (Linear Regression, Model Evaluation)

## 📂 Dataset
The dataset comprises ~550,000 observations with features including:
* User Demographics (Age, Gender, Occupation, Marital Status)
* City Category & Stay Duration
* Product Categories (Masked Category 1, 2, 3)

## 📊 Results
* **Model Used:** Linear Regression
* **Metric:** R2 Score (Coefficient of Determination)
* **Output:** The model successfully predicts purchase values and provides interpretable coefficients for business strategy.
