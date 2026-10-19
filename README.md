# Predict Salary Based on Years of Experience

A Machine Learning project using **Linear Regression** and **Polynomial Regression** to predict an employee's salary (in LPA) based on their years of experience.

## 📌 Project Overview

This project analyzes a real-world, noisy dataset (`polynomial_regression_salary_dirty_500.csv`) containing records of employee experience, salary, department, education level, and location. It implements an end-to-end data science pipeline:
- **Data Inspection & Cleaning**: Handling missing values (`NaN`), imputing experience values, and removing corrupted target records.
- **Outlier Detection & Filtering**: Identifying and removing invalid records (such as negative experience, negative salary, and extreme anomalies).
- **Feature Scaling**: Standardizing features using `StandardScaler`.
- **Model Training & Comparison**:
  - **Simple Linear Regression**: Baseline linear fit.
  - **Polynomial Regression**: Fitting polynomial curves to capture non-linear trends in salary growth with increasing experience.
- **Interactive Prediction**: Custom salary prediction for any input years of experience.

## 📂 Repository Contents

```
├── Predict_Salary.ipynb                       # Main Jupyter Notebook with data cleaning, EDA, and models
├── polynomial_regression_salary_dirty_500.csv # Dataset used for training and evaluation
├── .gitignore                                 # Git ignore rules for checkpoints and OS metadata
└── README.md                                  # Project documentation
```

## 🛠️ Requirements & Installation

Make sure you have Python 3.8+ installed along with the required libraries:

```bash
pip install numpy pandas scikit-learn matplotlib
```

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/arnavmhetre1806-cmd/Predict-Salary.git
   cd Predict-Salary
   ```

2. Launch Jupyter Notebook or Jupyter Lab:
   ```bash
   jupyter notebook Predict_Salary.ipynb
   ```

3. Run the cells sequentially to execute the data cleaning pipeline, visualize the regression models, and test predictions.

## 📊 Results Summary

- Polynomial regression provides a significantly better fit compared to simple linear regression by capturing non-linear salary growth as seniority increases.
- Data cleaning steps (removing negative values and extreme outliers) are crucial for model accuracy and stability.
