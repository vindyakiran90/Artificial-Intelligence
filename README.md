# 🔷 Linear Algebra – Day 04 Assignment  
**Topic:** Spectral Clustering using Graph Laplacian and Eigen Decomposition  

**Author:** Vindya Kiran Jain  
**File:** `Day_04_Linear_Algebra_Assignment_Vindya_Kiran_Jain.ipynb`  
**Course:** Artificial Intelligence & Machine Learning  
**Module:** Linear Algebra for AI
---

## 📘 Overview

This notebook explores **Spectral Clustering**, a graph-based clustering algorithm that utilizes **eigenvalues** and **eigenvectors** of a **graph Laplacian** to detect complex, non-linearly separable clusters.  

Unlike traditional algorithms like *k-means*, which assume convex clusters in Euclidean space, spectral clustering leverages **graph theory and linear algebra** to uncover intrinsic data structures.

---

## 🧩 Key Concepts

### 1️⃣ Similarity Graph
- Represents data points as **nodes** and their pairwise relationships as **edges**.
- Edge weights represent **similarity** between data points (often computed via Gaussian RBF kernel).

### 2️⃣ Degree Matrix (D)
- A diagonal matrix where each diagonal element represents the **sum of edge weights** connected to a node.

### 3️⃣ Graph Laplacian (L)
\[
L = D - W
\]
Where:
- **D** = Degree matrix  
- **W** = Adjacency (similarity) matrix  

The Laplacian captures the structure of the graph and is crucial for understanding cluster connectivity.

### 4️⃣ Eigen Decomposition
- Eigenvalues and eigenvectors of \( L \) provide insights into the **connected components** of the graph.  
- The smallest eigenvalues correspond to **smooth variations** across clusters.

### 5️⃣ Spectral Embedding
- The top \( k \) eigenvectors (smallest non-zero eigenvalues) are used to **embed data points** into a lower-dimensional space.

### 6️⃣ Clustering in Embedded Space
- After embedding, **k-means** or another clustering algorithm is applied to the transformed data to obtain final clusters.

---
