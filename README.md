# 🤖 Machine Learning – Day 3 Assignment  
**Topic:** Regularization and Regression Model Comparison  

**Author:** Vindya Kiran Jain  
**File:** `ML_Day_03.ipynb`  
**Course:** Artificial Intelligence & Machine Learning  
**Module:** Machine Learning

---

## 📘 Overview

This notebook explores **Regularization techniques in Machine Learning** and compares various **Regression models** using the **California Housing dataset**.  

It demonstrates how **L1 (Lasso)**, **L2 (Ridge)**, and **Elastic Net** regularizations help reduce **overfitting**, improve **model generalization**, and manage **multicollinearity** among predictors.

---

## 🧩 Objectives

1. Understand and implement **regularization** techniques:
   - L1 Regularization (**Lasso Regression**)
   - L2 Regularization (**Ridge Regression**)
   - Combined Regularization (**Elastic Net**)
2. Compare performance with standard **Linear Regression** and **Decision Tree Regression**.
3. Evaluate models using key metrics and visualize results.

---

## 📂 File Description

| File Name | Description |
|------------|-------------|
| `ML_Day_03.ipynb` | Jupyter Notebook containing all code, visualizations, and analysis for regression model comparison. |
| `california_housing.csv` | Dataset used for model training and evaluation (loaded from `sklearn.datasets`). |

---

## 🧮 Concepts Covered

### 🔹 Regularization Overview
- Prevents **overfitting** by penalizing large coefficients.
- Improves **model stability** and **generalization**.

| Technique | Penalty Term | Effect |
|------------|---------------|--------|
| **L1 (Lasso)** | `λ * Σ|wᵢ|` | Performs feature selection (sets some coefficients to 0). |
| **L2 (Ridge)** | `λ * Σwᵢ²` | Shrinks coefficients but retains all features. |
| **Elastic Net** | Combination of L1 + L2 | Balances selection and shrinkage. |

---

## 🧠 Models Implemented

1. **Linear Regression (Baseline)**  
2. **Lasso Regression (L1 Regularization)**  
3. **Ridge Regression (L2 Regularization)**  
4. **Elastic Net Regression (L1 + L2 Regularization)**  
5. **Decision Tree Regression (Non-linear model)**  

Each model is trained, tested, and evaluated on the **California Housing Dataset**.

---

## ⚙️ Implementation Steps

### 1️⃣ Data Loading & Preprocessing
- Loaded California Housing dataset from `sklearn.datasets`.  
- Split data into train/test sets (80/20).  
- Performed scaling and feature normalization.  

### 2️⃣ Model Training
- Trained five regression models with and without regularization.  
- Tuned hyperparameters such as:
  - `alpha` (regularization strength)
  - `max_depth` (for Decision Tree)

### 3️⃣ Evaluation Metrics
| Metric | Description | Ideal |
|---------|--------------|-------|
| **R² Score** | Variance explained by model | Closer to 1 |
| **RMSE** | Root Mean Square Error | Lower is better |
| **MAE** | Mean Absolute Error | Lower is better |

---

## 📊 Sample Results

| Model | R² Score | RMSE | Remarks |
|--------|-----------|------|----------|
| Linear Regression | 0.61 | 0.72 | Baseline model |
| Lasso Regression | 0.59 | 0.75 | Slight underfit due to high penalty |
| Ridge Regression | 0.62 | 0.71 | Improved stability |
| Elastic Net | 0.61 | 0.73 | Balanced performance |
| Decision Tree | 0.78 | 0.58 | Strong performance but prone to overfitting |

---

## 🧾 Key Insights

- Regularization helps control overfitting in linear models.  
- **Ridge Regression** provided a balanced bias-variance tradeoff.  
- **Lasso** eliminated weak features, improving interpretability.  
- **Decision Tree Regression** performed best but requires depth control.  
- **Elastic Net** worked well when both feature selection and shrinkage were needed.

---

## 🛠️ Tools & Libraries Used

- **Python 3.x**
- **Pandas**, **NumPy**
- **Matplotlib**, **Seaborn**
- **Scikit-learn**

---

## 🚀 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/vindyakiran90/Artificial-Intelligence.git
