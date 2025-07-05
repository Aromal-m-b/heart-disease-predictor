# heart-disease-predictor
A machine learning-based system for predicting heart disease risk using key clinical features. Supports multiple models like Logistic Regression, Random Forest, and XGBoost. Offers user input, model selection, and human-readable output for better diagnosis.

# 🩺 Heart Disease Predictor

A machine learning-based system for predicting heart disease risk using key clinical features. This project enables users to input important medical values and select from multiple pre-trained ML models to determine the probability and severity of heart disease.

---

## 📌 Overview

Heart disease is one of the leading causes of death globally. Early diagnosis significantly increases the chances of effective treatment. This project uses machine learning models to predict the risk of heart disease based on three key features:

- `ca`: Number of major vessels (0–3) detected by fluoroscopy
- `thal`: Thalassemia test result (1 = normal, 2 = fixed defect, 3 = reversible defect)
- `oldpeak`: ST depression induced by exercise

---

## ✅ Features

### 🔹 User-Friendly Input Interface
Users are prompted to enter:
- **ca**: Number of major vessels (0 to 3)
- **thal**: Thalassemia result (1, 2, or 3)
- **oldpeak**: ST depression (float, e.g., 1.4)

This makes the system usable in CLI or GUI setups.

### 🔹 Multiple Model Support
The project supports real-time model selection:
- `logistic`: Logistic Regression
- `knn`: K-Nearest Neighbors
- `random_forest`: Random Forest
- `xgboost`: XGBoost (recommended for best accuracy)

Users can type the model name to switch dynamically.

### 🔹 Human-Readable Output
Model predictions (numerical values) are translated into understandable labels:

| Prediction | Diagnosis               |
|------------|-------------------------|
| 0          | No heart disease        |
| 1          | Low risk                |
| 2          | Medium risk             |
| 3          | High risk               |
| 4          | Very high risk          |

### 🔹 Class Imbalance Handling
Real-world data is often imbalanced. The system handles this by:
- Using `class_weight='balanced'` in certain models
- Supporting SMOTE (Synthetic Minority Over-sampling Technique)

This ensures the model treats all classes fairly.

### 🔹 Overfitting Prevention
Techniques used to reduce overfitting:
- Hyperparameter tuning (`max_depth`, `learning_rate`, `n_estimators`)
- Early stopping in boosting models
- Validation accuracy tracking alongside training accuracy

### 🔹 Modular and Extensible Code
- Easily add new models
- Clean separation of logic for data input, model selection, and prediction
- Can be extended into web apps or APIs

---
## 📈 Model Performance Summary

| Model           | Train Accuracy | Test Accuracy | Remarks                |
|----------------|----------------|---------------|------------------------|
| Logistic        | 76%            | 50%           | Good baseline model    |
| K-Nearest Neighbors (KNN) | 65%            | 49%           | Underfitting observed |
| Random Forest   | 70%            | 50%           | Risk of overfitting    |
| XGBoost         | 76%            | 50%           | Best performance so far|

---

## ⚙️ Tech Stack

- **Python 3.8+**
- **scikit-learn** – machine learning algorithms
- **XGBoost** – gradient boosting classifier
- **imbalanced-learn** – SMOTE for class balancing
- **NumPy & Pandas** – data manipulation
- **Matplotlib & Seaborn** – visualization
- **Jupyter Notebook** – development environment

---
## 🧰 Installation & Usage

For complete setup instructions and how to run the project, see the  
📄 [Installation and Usage Guide](./installation-and-usage-guide.md)
