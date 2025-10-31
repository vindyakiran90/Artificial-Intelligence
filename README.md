# 🔢 Linear Algebra – Day 01 Assignment  
**Topic:** Gradient Descent vs Adam Optimizer  

**Author:** Vindya Kiran Jain  
**File:** `Day_01_Linear_Algebra_Assignment_AI10_Vindya_Kiran_Jain.ipynb`  
**Course:** Artificial Intelligence & Machine Learning  
**Module:** Linear Algebra for AI  
**Date:** [Insert Submission Date]

---

## 📘 Overview

This assignment explores **optimization techniques** used in **Linear Regression**, comparing the performance of **Vanilla Gradient Descent** and the **Adam Optimizer**.  

Both methods are applied to a **synthetic dataset**, and their convergence patterns are analyzed through visualizations and error metrics.

---

## 🧩 Objectives

1. Implement **Linear Regression** from scratch using **NumPy**.  
2. Compare **Vanilla Gradient Descent** with **Adam Optimizer**.  
3. Visualize and analyze model convergence behavior.  
4. Summarize performance, stability, and efficiency observations.

---

## 📂 File Description

| File Name | Description |
|------------|-------------|
| `Day_01_Linear_Algebra_Assignment_AI10_Vindya_Kiran_Jain.ipynb` | Jupyter Notebook implementing Linear Regression using both Gradient Descent and Adam optimization algorithms. |

---

## ⚙️ Implementation Details

### **1️⃣ Dataset**
- A synthetic dataset is generated using NumPy:
  \[
  y = 3x + 7 + \text{noise}
  \]
- 400 samples with Gaussian noise.

### **2️⃣ Model**
- Linear Regression Model:  
  \[
  \hat{y} = w_1x + w_0
  \]
- Loss Function: **Mean Squared Error (MSE)**

---

## 🚀 Gradient Descent Variants Implemented

### **🧮 Vanilla Gradient Descent**
- Fixed learning rate = `0.01`  
- Updates weights in the direction of the negative gradient.  
- Slower convergence, sensitive to learning rate.  

### **⚡ Adam Optimizer**
- Adaptive learning rates using **momentum** and **RMSProp**.  
- Hyperparameters:
  - Learning Rate: `0.05`
  - β₁ = 0.9, β₂ = 0.999, ε = 1e-8
- Converges faster and more stable for noisy gradients.

---
