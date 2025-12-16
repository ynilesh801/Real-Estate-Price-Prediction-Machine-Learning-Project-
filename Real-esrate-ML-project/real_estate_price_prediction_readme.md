# 🏠 Real Estate Price Prediction (Machine Learning Project)

## 1. Project Overview

This project demonstrates a complete **end-to-end Machine Learning workflow** using a real-world dataset to predict **house prices** based on area-level features.

The goal of this project is not just to train a model, but to understand **how Machine Learning works step by step**, starting from raw data and ending with a trained and evaluated model.

This is a **regression-based ML project** and is designed as a **first, foundational ML project**.

---

## 2. Problem Statement

Given information about a residential area such as:
- Average income of the area
- Average house age
- Number of rooms and bedrooms
- Area population

Predict the **price of a house** in that area.

### Problem Type
- **Regression** (because the output is a continuous numerical value)

### Target Variable
- `Price`

---

## 3. Dataset Description

**Dataset Name:** Real Estate Dataset  
**Format:** CSV file  

### Dataset Columns

| Column Name | Description |
|------------|------------|
| Avg. Area Income | Average income of people living in the area |
| Avg. Area House Age | Average age of houses in the area |
| Avg. Area Number of Rooms | Average number of rooms per house |
| Avg. Area Number of Bedrooms | Average number of bedrooms per house |
| Area Population | Population of the area |
| Price | House price (Target Variable) |
| Address | Address of the property (not used in modeling) |

The dataset is clean and does not contain missing values.

---

## 4. Exploratory Data Analysis (EDA)

Before building the model, basic data exploration was performed to:
- Understand data structure and data types
- Identify numerical and non-numerical columns
- Check for missing values
- Review basic statistical properties

The `Address` column was identified as non-informative for prediction and removed during preprocessing.

---

## 5. Feature Selection

### Features Used (X)
- Avg. Area Income
- Avg. Area House Age
- Avg. Area Number of Rooms
- Avg. Area Number of Bedrooms
- Area Population

### Target (y)
- Price

The `Address` column was excluded as Machine Learning models require numerical inputs and it does not provide predictive value in this context.

---

## 6. Train-Test Split

The dataset was split into:
- **80% Training Data** (used to train the model)
- **20% Testing Data** (used to evaluate the model)

This ensures that the model is tested on unseen data and does not memorize the dataset.

---

## 7. Model Used

### Linear Regression

A **Linear Regression model** was chosen as the baseline model because:
- It is simple and interpretable
- It is ideal for regression problems
- It helps understand relationships between features and target

The model learns a linear relationship between input features and the house price.

---

## 8. Model Training

The model was trained using the training dataset after separating features and target variables.

The model learned coefficients for each feature that represent their contribution to house price prediction.

---

## 9. Model Evaluation

The model was evaluated using the following metrics:

### Mean Absolute Error (MAE)
- Measures the average absolute difference between predicted and actual prices
- Easy to interpret in real-world terms

### R² Score (Coefficient of Determination)
- Measures how much variance in house prices is explained by the model

### Results
- **MAE:** Approximately 80,000
- **R² Score:** Approximately 0.92

This indicates that the model explains around **92% of the variation** in house prices, which is a strong result for a baseline regression model.

---

## 10. Model Interpretation

The coefficients of the Linear Regression model were analyzed to understand feature importance.

Key observations:
- Average Area Income has a strong positive impact on house price
- Number of rooms significantly influences price
- Area population and house age also contribute to predictions

This makes the model transparent and explainable.

---

## 11. Conclusion

- A complete Machine Learning pipeline was successfully implemented
- Proper data preparation and feature selection led to strong performance
- Linear Regression proved effective for this dataset
- The project demonstrates a solid understanding of core ML concepts

This project serves as a strong **beginner-level Machine Learning project**.

---

## 12. Project Structure

```
real-estate-ml-project/
│
├── data/
│   └── Real_estates.csv
├── notebook/
│   └── house_price_prediction.ipynb
├── README.md
```

---

## 13. Tools & Libraries Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Jupyter Notebook

---

## 14. Future Improvements

- Try additional regression models (Ridge, Lasso)
- Perform cross-validation
- Analyze residual plots
- Add feature scaling and normalization

---

## 15. Author
**Nilesh Yadav**
This project was created as a **learning-focused Machine Learning project** to understand the complete ML workflow from start to end.

---

