# 📊 Statistics for Artificial Intelligence — Assignment

**Author:** Vindya Kiran Jain  
**File:** `Statistics_Assignment_Vindya_Kiran_Jain.ipynb`  
**Course:** Artificial Intelligence  
**Module:** Statistical Foundations for AI

---

## 📘 Overview

This assignment explores **statistical data analysis** using the **HR Employee Attrition dataset**.  
The focus is on applying **parametric and non-parametric hypothesis testing techniques** to understand the relationships between employee features such as age, income, and job satisfaction.

---

## 🧾 Objectives

1. Identify whether numerical variables follow a **normal distribution**.  
2. Apply suitable **parametric (t-test, ANOVA)** or **non-parametric (Mann-Whitney U, Kruskal-Wallis)** tests based on data characteristics.  
3. Formulate and test **null and alternative hypotheses** for binary and multi-group comparisons.  
4. Interpret statistical test results to draw meaningful conclusions.

---

## 📂 File Description

| File Name | Description |
|------------|--------------|
| `Statistics_Assignment_Vindya_Kiran_Jain.ipynb` | Jupyter Notebook containing the statistical analysis, visualizations, and hypothesis testing results. |
| `WA_Fn-UseC_-HR-Employee-Attrition.csv` | Dataset used for employee attrition analysis. |

---

## 🧩 Assignment Structure

### **1️⃣ Data Import and Cleaning**
- Imported HR Attrition dataset using Pandas.  
- Selected relevant columns:
  - `Age`, `MonthlyIncome`, `JobSatisfaction`, `Attrition`, `JobRole`
- Cleaned missing values, removed duplicates, and stripped extra spaces.

---

### **2️⃣ Part A — Parametric or Non-Parametric?**
- Checked normality of numeric variables (`MonthlyIncome`, `Age`) using:
  - **Histograms**  
  - **Boxplots**  
  - **Q–Q plots**
  - **Shapiro-Wilk** and **Kolmogorov–Smirnov tests**
- Decided the statistical test type (parametric / non-parametric) based on results.

---

### **3️⃣ Part B — Hypothesis Test (Binary Group)**
**Example Hypothesis:**
- **H₀:** There is no difference in Monthly Income between employees who left and those who stayed.  
- **H₁:** There is a difference between the two groups.

Tests Used:
- ✅ Independent Two-Sample **t-test** (if normal)
- ✅ **Mann–Whitney U Test** (if non-normal)

---

### **4️⃣ Part C — Hypothesis Test (Multiple Groups)**
**Example Hypothesis:**
- **H₀:** The median job satisfaction is the same across all job roles.  
- **H₁:** At least one job role differs in median job satisfaction.

Tests Used:
- ✅ **One-way ANOVA** (if normal)  
- ✅ **Kruskal–Wallis Test** (if non-normal)

---

### **5️⃣ Data Visualization**
- Histograms and Boxplots to observe data distribution.  
- Q-Q plots using **Statsmodels**.  
- Visual comparisons across attrition and job role groups using **Seaborn**.

---

## 🧠 Libraries Used

- **Python 3.x**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **SciPy**
- **Statsmodels**

---
