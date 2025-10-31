# 🤖 Machine Learning – Day 1 Assignment  
**Topic:** Life Expectancy Prediction using Linear Regression  

**Author:** Vindya Kiran Jain  
**File:** `ML_Day_01_Assignment_Vindya_Kiran_Jain.ipynb`  
**Course:** Artificial Intelligence & Machine Learning  
**Module:** Machine Learning

---

## 📘 Overview

This assignment focuses on building and evaluating a **Linear Regression model** to predict **Life Expectancy** based on various socio-economic and health-related features.

The notebook demonstrates:
- Data loading and preprocessing  
- Feature selection and engineering  
- Model training and evaluation  
- Interpretation of results and key insights  

---

## 📂 File Description

| File Name | Description |
|------------|-------------|
| `ML_Day_01_Assignment_Vindya_Kiran_Jain.ipynb` | Main Jupyter Notebook containing model implementation, results, and discussion. |
| `Life_Expectancy_Data.csv` | Dataset used for analysis and model training. *(If applicable)* |

---

## 🧩 Key Tasks

### **1️⃣ Data Preparation**
- Imported and cleaned the **Life Expectancy dataset**.  
- Handled missing values and irrelevant columns.  
- Performed feature engineering to prepare predictors and target variable (`life_expectancy`).  

---

### **2️⃣ Model Building**
- Built a **Linear Regression model** using scikit-learn.  
- Split data into **training** and **testing** sets.  
- Trained the model and generated predictions on test data.  

---

### **3️⃣ Model Evaluation**

#### 📈 Metrics Used:
| Metric | Meaning | Goal |
|---------|----------|------|
| **R² Score** | Proportion of variance explained by the model | Closer to 1 |
| **RMSE (Root Mean Squared Error)** | Average prediction error (in years) | Lower is better |

#### 📊 Results:
| Metric | Value | Interpretation |
|---------|--------|----------------|
| **R² Score** | **0.806** | ~80.6% of Life Expectancy variance explained |
| **RMSE** | **4.15 years** | Predictions deviate by ~4.15 years on average |

---

## 🔍 Insights

### ✅ Strengths
- High **R² score (0.806)** indicates a strong model fit.  
- Model is simple and **highly interpretable**.  
- Identifies key socio-economic factors affecting life expectancy.

### ❌ Limitations
- **Linear assumptions** may not capture complex relationships.  
- Sensitive to **outliers** and **multicollinearity**.  
- Moderate prediction error (**RMSE = 4.15** years).

---

## 💡 Best Predictors Identified

| Feature | Description | Relationship |
|----------|--------------|---------------|
| **Adult Mortality** | Mortality rate among adults | Negative |
| **Schooling** | Average years of education | Positive |
| **HIV/AIDS** | Death rate due to HIV/AIDS | Negative |
| **Income Composition** | Income inequality measure | Positive |
| **BMI** | Average body mass index | Positive |

---

## 🛠️ Tools & Libraries Used

- **Python 3.x**  
- **Pandas** – Data manipulation  
- **NumPy** – Numerical operations  
- **Matplotlib / Seaborn** – Visualization  
- **Scikit-learn** – Model building and evaluation  

---
