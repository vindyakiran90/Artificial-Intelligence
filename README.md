# 💻 Python Programming – Assignment 02  

**Author:** Vindya Kiran Jain  
**File:** `Assignment_02.ipynb`  
**Course:** Artificial Intelligence & Machine Learning  
**Module:** Programming Essentials for AI

---

## 📘 Overview

This notebook demonstrates advanced Python programming concepts, focusing on:
- **File handling**
- **Object-Oriented Programming (OOP)**
- **Custom exceptions**
- **Iterators and Generators**
- **Multiple inheritance**

Each section applies these concepts through practical, well-structured programs.

---

## 📂 File Description

| File Name | Description |
|------------|-------------|
| `Assignment_02.ipynb` | Jupyter Notebook containing all five Python programming tasks with code, logic, and execution results. |
| `students.json` | Example data file for Task 1 (JSON-based student records). |
| `data.csv` | Example CSV file for Task 3 (FileManager demonstration). |

---

## 🧩 Tasks Breakdown

### **1️⃣ Working with Sequences and JSON**
**Objective:**  
- Read a JSON file containing a list of students and their grades.  
- Sort students based on their **average grade**.  
- Handle malformed files or missing data gracefully.  
- Write the sorted data back to a new JSON file.

**Concepts Used:**  
- JSON file handling  
- Python list and dictionary operations  
- Exception handling  
- Sorting and sequence manipulation  

---

### **2️⃣ Exception Handling and User-defined Exceptions**
**Objective:**  
Develop a simple **banking application** that:  
- Allows users to **deposit** and **withdraw** money.  
- Raises exceptions for:
  - Negative input  
  - Insufficient funds  
  - Invalid account operations  
- Implements **custom exception classes** for better control.

**Concepts Used:**  
- Custom exceptions (`class InsufficientFundsError(Exception):`)  
- `try-except` blocks  
- Error propagation and validation  

---

### **3️⃣ File Operations and Object-Oriented Design**
**Objective:**  
Create a **FileManager class** to handle CSV and text file operations.

**Features:**
- Read and write file data.  
- Use of **private variables** and **class methods**.  
- Implement **inheritance** for handling multiple file types (e.g., TextFileManager, CSVFileManager).  
- Include **error handling** and **method documentation**.

**Concepts Used:**  
- OOP principles (Encapsulation, Inheritance)  
- File handling  
- Polymorphism  

---

### **4️⃣ Iterators and Generators**
**Objective:**  
Implement a **custom iterable class** that generates Fibonacci numbers up to a limit.

**Included Implementations:**
- A class implementing `__iter__()` and `__next__()`  
- A **generator function** using `yield`  
- A **generator expression** for concise syntax  
- Comparison of readability and performance

**Concepts Used:**  
- Iterators and Generators  
- Lazy evaluation  
- Pythonic performance comparison  

---

### **5️⃣ Advanced Class Design and Multiple Inheritance**
**Objective:**  
Design a **role-based access control (RBAC)** system using classes like `User`, `Admin`, and `Guest`.

**Features:**
- Shared and role-specific functionalities.  
- Use of **multiple inheritance** for permission management.  
- Implementation of **method overriding** and **polymorphism**.  
- Track user state using **class and instance variables**.

**Concepts Used:**  
- Multiple inheritance  
- Method overriding  
- Polymorphism  
- Docstrings and error handling  

---

## 🧠 Key Learnings

✅ Advanced Python OOP principles  
✅ Exception handling and user-defined errors  
✅ JSON and CSV file management  
✅ Iterators, generators, and performance optimization  
✅ Multiple inheritance and polymorphism  

---

## 🛠️ Libraries Used

- **Python 3.x**  
- **Pandas** *(optional for file handling)*  
- **JSON**  
- **CSV**  
- **OS** *(for file management)*  

---

## 🚀 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/vindyakiran90/Artificial-Intelligence.git
