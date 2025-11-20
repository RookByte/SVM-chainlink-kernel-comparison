# SVM_Kernel_Comparison_Chainlink💡
=======
# Support Vector Machine Kernel Comparison on 3D Chainlink Dataset

This repository demonstrates the **power of non-linear kernels** in Support Vector Machines using the famous **Chainlink** dataset — a classic example of data that is **not linearly separable** in 3D space.

---

## Overview⚡

- **Dataset:** `chainlink.csv` – 1000 synthetic 3D points forming two intertwined rings  
- **Features:** `x`, `y`, `z`  
- **Target:** `class` (0 or 1)  
- **Model:** Support Vector Classifier (`SVC`)  
- **Kernels Compared:** `linear` vs `rbf` (Gaussian)  
- **Visualization:** Interactive 3D scatter plots using Matplotlib (`%matplotlib qt`)

---

## Method⭐

1. Load the Chainlink dataset and explore the 3D structure.  
2. Visualize the **original labeled data** in 3D — two clearly intertwined rings.  
3. Split into **train (80%)** and **test (20%)** sets.  
4. Train two SVC models:
   - `kernel='linear'` → expected to fail
   - `kernel='rbf'` → uses the **Kernel Trick** to separate non-linear patterns  
5. Predict on test set and visualize predictions in 3D.  
6. Compare how each kernel handles the non-linear decision boundary.

## Results🔍

| Kernel   | 3D Separation Quality       
|----------|-----------------------------
| linear   | Complete failure — classes mixed 
| rbf      | Near-perfect separation     

**Key Insight:**  
Even though no straight line (or plane) can separate the rings in 3D, the **RBF kernel** maps the data to a higher-dimensional space where separation becomes trivial — this is the **Kernel Trick** in action!

## 3D Visualizations🔗

- Original data: Two beautiful intertwined rings  
- Linear kernel: Predictions are random — model cannot learn the pattern  
- RBF kernel: Almost perfect classification — rings cleanly separated

## Skills Demonstrated⚙️

- 3D data visualization with Matplotlib
- Deep understanding of **linear separability** and the **Kernel Trick**
- Practical comparison of SVM kernels
- Clean, reproducible ML experimentation

Perfect portfolio piece for **Machine Learning**, **Data Science**, or **Interview Preparation**.

---

Made with passion for understanding how things really work✨
