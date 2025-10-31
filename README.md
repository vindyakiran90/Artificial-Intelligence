# 🌲 Machine Learning – Day 4 Assignment  
**Topic:** Random Forest Regression & Hyperparameter Optimization  

**Author:** Vindya Kiran Jain  
**File:** `ML_Day_04.ipynb`  
**Course:** Artificial Intelligence & Machine Learning  
**Module:** Machine Learning

---

## 📘 Overview

This assignment focuses on implementing a **Random Forest Regression model** to predict continuous outcomes and applying **RandomizedSearchCV** for hyperparameter optimization.

The project demonstrates:
- Understanding ensemble learning with Random Forests  
- Parameter tuning for model improvement  
- Model evaluation using regression metrics  
- Visualization of feature importance  

---

## 📂 File Description

| File Name | Description |
|------------|-------------|
| `ML_Day_04.ipynb` | Jupyter Notebook implementing Random Forest Regression and RandomizedSearchCV. |
| `california_housing.csv` *(optional)* | Dataset used for regression (from `sklearn.datasets`). |

---

## 🧩 Key Concepts Covered

### **1️⃣ Random Forest Regression**
- Ensemble of multiple **Decision Trees** trained on random subsets of data and features.
- Combines predictions through **averaging** for better generalization.

#### 🧠 Why Random Forest?
✅ Handles both linear and non-linear data  
✅ Reduces overfitting  
✅ Provides feature importance  
✅ Works well with missing and noisy data  

#### ⚙️ Main Hyperparameters
| Parameter | Description |
|------------|--------------|
| `n_estimators` | Number of trees in the forest |
| `max_depth` | Maximum depth of trees |
| `min_samples_split` | Minimum samples required to split a node |
| `min_samples_leaf` | Minimum samples required at a leaf |
| `max_features` | Number of features to consider for best split |
| `bootstrap` | Whether to use bootstrap sampling |

---

### **2️⃣ RandomizedSearchCV – Hyperparameter Optimization**
- Randomly samples combinations of hyperparameters for tuning.  
- Faster alternative to exhaustive **GridSearchCV**.  

#### 🧠 How It Works:
1. Define the model (e.g., `RandomForestRegressor`)  
2. Provide parameter distributions  
3. Randomly sample N combinations  
4. Train and evaluate models  
5. Return best parameter set  

#### Example Code Snippet:
```python
from sklearn.model_selection import RandomizedSearchCV
from sklearn.ensemble import RandomForestRegressor

rf = RandomForestRegressor()
param_dist = {
    'n_estimators': [50, 100, 200, 300],
    'max_depth': [5, 10, 15, 20, None],
    'min_samples_split': [2, 5, 10],
    'min_samples_leaf': [1, 2, 4],
    'max_features': ['auto', 'sqrt']
}

rf_random = RandomizedSearchCV(estimator=rf, param_distributions=param_dist, 
                               n_iter=20, cv=5, random_state=42, n_jobs=-1)
rf_random.fit(X_train, y_train)
