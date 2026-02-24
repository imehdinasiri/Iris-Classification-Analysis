# 🌸 Iris Species Classification: Comparative Analysis

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/imehdinasiri/Iris-Classification-Analysis/blob/main/Iris_classification_analysis.ipynb)

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)

## 📋 Overview
This repository contains a structured comparative evaluation of seven supervised classification algorithms on the classic Fisher's **Iris dataset**. We evaluate model performance across probabilistic, linear, nonlinear, instance-based, and ensemble learning paradigms. 

The project also investigates the effect of **Principal Component Analysis (PCA)** for dimensionality reduction and visualization of the feature space.

## 🛠 Methodology
* **Dataset:** Iris (150 samples, 4 features).
* **Preprocessing:** Data was standardized and split into **80% Training** and **20% Testing** sets.
* **Dimensionality Reduction:** PCA applied for 2D visualization of class separability.

## 🤖 Evaluated Models
1. **Logistic Regression (LR)**
2. **Support Vector Machine (SVM)**
3. **Random Forest (RF)**
4. **K-Nearest Neighbors (KNN)**
5. **Linear Discriminant Analysis (LDA)**
6. **Quadratic Discriminant Analysis (QDA)**
7. **Gaussian Naive Bayes (GNB)**

## 📊 Results Summary
Based on the experimental results on the independent test split:

| Model | Test Accuracy | Paradigm |
| :--- | :---: | :--- |
| **Logistic Regression** | **100%** | Linear |
| **SVM (RBF Kernel)** | **100%** | Non-linear / Kernel |
| **Random Forest** | **100%** | Ensemble |
| **KNN (k=5)** | **100%** | Instance-based |
| **LDA** | **100%** | Linear / Generative |
| **QDA** | **~96.0%** | Non-linear / Generative |
| **Gaussian NB** | **~93.3%** | Probabilistic |

## 🧠 Discussion & Key Takeaways
* **Linear Separability:** Classical linear models (LR, SVM, LDA) achieved perfect classification, demonstrating that the Iris dataset is readily separable in the chosen feature representation.
* **Model Assumptions:** Gaussian Naive Bayes obtained lower accuracy (≈93.33%) due to its strong assumptions regarding feature distributions that do not fully match the empirical data. QDA (96%) likely suffers from covariance estimation variability on this small dataset.
* **Bias–Variance Interpretation:** The negligible train/test gap for the top models indicates low variance. However, perfect test accuracy can be misleading—it often reflects a favorable random split or dataset simplicity rather than absolute model superiority. 
* **Conclusion:** For low-dimensional, well-structured datasets, simple linear models are highly sufficient; ensemble or kernel methods provide additional robustness but not necessarily superior generalization in this specific case.

## 🚀 How to Run
You can run this project in two ways:

### 1. Instant Execution (Cloud)
The easiest way to explore the analysis is to run it directly in your browser via Google Colab. Click the button below to start:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/imehdinasiri/Iris-Classification-Analysis/blob/main/iris_classification_analysis.ipynb)
*This will open a private copy of the notebook for you to execute.*

### 2. Local Execution
If you prefer to run it on your machine:
1. Clone the repository:
   ```bash
   git clone [https://github.com/YourUsername/YourRepoName.git](https://github.com/imehdinasiri/Iris-Classification-Analysis.git)
2. Install the necessary libraries: pip install pandas numpy matplotlib scikit-learn


3. Open the notebook using Jupyter: jupyter notebook iris_classification_analysis.ipynb
