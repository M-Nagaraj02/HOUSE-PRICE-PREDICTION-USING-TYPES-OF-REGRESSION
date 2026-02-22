# 🏠 House Price Prediction using Regression Models
---
## 📌 Overview

This project demonstrates different types of Regression Algorithms used for predicting house prices.
The project covers:
 * Simple Linear Regression
 * Multiple Linear Regression
 * Polynomial Regression
The dataset is synthetically generated using NumPy and includes features like:

* Area
* Bedrooms
* Age
* Price
The objective is to understand how different regression models perform and compare their results.
---
## 📊 Dataset
The dataset is artificially generated using NumPy.
Features:

* area – Size of house (sq.ft)
* bedrooms – Number of bedrooms
* age – Age of the house
* price – Target variable
```python
import numpy as np
import pandas as pd
```
* Total Records: 100
* Total Features: 3
* Target Variable: Price
---
# 📈 Types of Regression Implemented
---
# 1️⃣ Simple Linear Regression

## 📌 Description

Implemented using scikit-learn ```LinearRegression()``` model.
Used only one independent feature (Age) to predict house price.

```python
X = df[["age"]]
Y = df["price"]
```
## 📊 Model Evaluation

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)
* R2 Score

**🔎 Results**

* MAE: 33.77
* MSE: 1549.20
* RMSE: 39.35
* R2 Score: -0.02
**📌 Insight**

* Poor performance
* Negative R² score
* Age alone is not sufficient to predict house price

## 📊 Visualizations

**Kde plot visualization of using Seaborn:**
<img width="480" height="393" alt="image" src="https://github.com/user-attachments/assets/fcecb1a8-fb89-48ca-9812-fc21468b8bd0" />

**Scatterplot visualization of using Matplotlib**
<img width="695" height="547" alt="image" src="https://github.com/user-attachments/assets/38b98d1f-3bb0-4447-b5a4-6cc12e51b4c9" />

---
# 2️⃣ Multiple Linear Regression
---
## 📌 Description

Used all features:

* Area
* Bedrooms
* Age
```python 
X = df[["area","bedrooms","age"]]
Y = df["price"]
```
## 📊 Model Evaluation
**🔎 Results**

* MAE: 8.47
* MSE: 99.70
* RMSE: 9.98
* R2 Score: 0.93
**📌 Insight**

* Excellent performance
* Strong relationship between features and price
* R² = 93% → Model explains most of the variance

**🏆 Best Performing Model**

Multiple Linear Regression performed significantly better than Simple Linear Regression.

## 📊 Visualizations

**Kde plot visualization of using Seaborn:**
<img width="500" height="393" alt="image" src="https://github.com/user-attachments/assets/3bd661ca-1f02-4e3f-83ba-c69fc027712f" />

**Scatterplot visualization of using Matplotlib:**
<img width="463" height="393" alt="image" src="https://github.com/user-attachments/assets/1bcdaec8-a043-4a9b-aa78-407143788be9" />

**Lineplot visualization of using Seaborn:**
<img width="463" height="393" alt="image" src="https://github.com/user-attachments/assets/171b94e6-ab84-443a-aeed-69ae23c620c2" />

---
# 3️⃣ Polynomial Regression
---
## 📌 Description

Used scikit-learn ```PolynomialFeatures``` with degree = 2.
```python
from sklearn.preprocessing import PolynomialFeatures
```

## 📊 Results

* R2 Score: 0.03

**📌 Insight**

* Slight improvement over Simple Linear Regression
* Still poor compared to Multiple Linear Regression
* Indicates relationship is more linear across multiple variables

## 📊 Visualizations

**Scatterplot visualization of using Matplotlib:**
<img width="463" height="393" alt="image" src="https://github.com/user-attachments/assets/cc4cd80f-6950-467e-9f49-300ffe5a0db0" />

---
## 📂 Project Structure
```
House-Price-Regression/
│── House_Price_Regression.ipynb
│── README.md
```
## 🧠 Key Concepts Demonstrated

* Supervised Machine Learning
* Regression Algorithms
* Train-Test Split
* Model Evaluation Metrics
* Overfitting vs Underfitting
* Feature Importance
* Polynomial Feature Engineering
---
## 📊 Performance Comparison

Model                        	R2 Score	Performance
Simple Linear Regression      	-0.02	      Poor
Multiple Linear Regression	     0.93   	Excellent
Polynomial Regression            0.03     	Weak

---
## 🚀 Skills Demonstrated

* Data Generation using NumPy
* Data Manipulation using Pandas
* Regression Modeling
* Error Metric Calculation
* Model Comparison
* Data Visualization using Matplotlib & Seaborn
* Machine Learning with Scikit-learn
---
## 👨‍💻 Author

**Nagaraj M**

GitHub: https://github.com/M-Nagaraj02
