## 📌 Task 7: AI & ML Internship Assignment  
# 💠 Breast Cancer Dataset - Support Vector Machines (SVM)

This repository contains a classification project using **SVM (Support Vector Machine)** algorithms with both **Linear** and **RBF** kernels on the Breast Cancer dataset. This task is part of the **AI & ML Internship** program and focuses on margin maximization, kernel tricks, hyperparameter tuning, and decision boundary visualization.

---

## 🎯 Objective  

To implement and compare Linear and RBF Kernel-based SVM models to:  
- Understand how SVM separates classes using optimal hyperplanes  
- Visualize margins and decision boundaries  
- Use the **kernel trick** to classify non-linearly separable data  
- Tune SVM hyperparameters (`C`, `gamma`) to improve generalization  
- Validate models using **cross-validation**

---

## 🧰 Tools and Libraries Used  

- Python  
- Jupyter Notebook / Google Colab  
- Pandas  
- NumPy  
- Matplotlib & Seaborn  
- Scikit-learn  

---

## 📂 Dataset  

The dataset used is the **Breast Cancer Wisconsin Dataset**, provided as `breast-cancer.csv`.  
It contains clinical features extracted from breast mass imagery to classify tumors as **benign (0)** or **malignant (1)**.

---

## 📊 What Was Done  

1. **Loaded and prepared the dataset**  
   - Handled missing/irrelevant columns  
   - Encoded the target column (`diagnosis`)  
   - Standardized features using `StandardScaler`  
   - Split data into training and testing sets  

2. **Trained a Support Vector Machine with Linear Kernel**  
   - Evaluated model performance  
   - Compared predictions with true labels  

3. **Trained a Support Vector Machine with RBF Kernel**  
   - Handled non-linear patterns more effectively  
   - Improved classification accuracy  

4. **Tuned Hyperparameters (`C` and `gamma`)**  
   - Used `GridSearchCV` for 5-fold cross-validation  
   - Found best `C` and `gamma` values  
   - Evaluated tuned model on test set  

5. **Evaluated using Cross-Validation**  
   - 5-fold cross-validation on the best model  
   - Verified stability and generalization capability  

6. **Visualized Decision Boundary using PCA**  
   - Reduced features to 2D using PCA  
   - Visualized SVM decision regions and class separations  

---

## 🔍 Key Insights  

- 🔹 **Linear SVM** worked well on separable data but showed limitations  
- 💡 **RBF Kernel SVM** captured complex decision boundaries  
- 🧪 **Tuned Model** gave the highest test and cross-validation accuracy  
- 🧠 **Cross-validation** confirmed the model's robustness  
- 🌀 **PCA-based plots** gave clear insights into margin boundaries

---

## 🧪 Results Summary  

| Model               | Test Accuracy | Cross-Validation Accuracy |
|--------------------|---------------|----------------------------|
| SVM (Linear Kernel) | 0.956         | —                          |
| SVM (RBF Kernel)    | 0.973         | —                          |
| SVM (Tuned RBF)     | **0.985**     | **0.982**                  |
