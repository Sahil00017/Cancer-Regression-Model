# Cancer-Regression-Model
📊 Analyzing and predicting cancer outcomes using regression models. This project leverages machine learning techniques to study cancer data and build predictive models for better insights.

# 🏥 Cancer Regression Analysis

## 📌 Project Overview

This project focuses on predicting cancer-related outcomes using various regression models. It involves **data preprocessing, feature engineering, and model evaluation** to find the best regression approach for accurate predictions.

### 🔬 Key Techniques Used:

- **Data Cleaning & Processing**
- **Feature Engineering & Transformation**
- **Exploratory Data Analysis (EDA)**
- **Multiple Regression Models**
- **Regularization Techniques (Lasso, Ridge, Elastic Net)**
- **Model Performance Evaluation using Metrics (MSE, RMSE, MAE, R² Score)**

---

## 📊 Dataset Description

The dataset contains multiple **features related to cancer diagnostics**, used to predict a key target variable.

**Key steps in data processing:**

- **Handling Missing Values** using median imputation.
- **Feature Encoding** for categorical variables.
- **Scaling & Normalization** to standardize the dataset.
- **Outlier Treatment** using **IQR Winsorization**.

---

## 📈 Regression Models & Performance

The following regression models were implemented and evaluated:

### 1️⃣ **Polynomial Regression**

- Captures non-linear relationships between features.
- **Issues:** Overfitting and instability in predictions.

### 2️⃣ **Regularized Regression Models**

Applied **Lasso, Ridge, and Elastic Net Regression** to prevent overfitting:

| Model                      | Training Accuracy | Testing Accuracy |
| -------------------------- | ----------------- | ---------------- |
| **Lasso Regression**       | 54.23%            | 53.48%           |
| **Ridge Regression**       | 54.82%            | 53.35%           |
| **Elastic Net Regression** | 54.38%            | 53.54%           |

### 3️⃣ **Tree-Based & Non-Linear Models**

Additional models tested for performance improvements:

| Model                         | Training Accuracy | Testing Accuracy |
| ----------------------------- | ----------------- | ---------------- |
| **K-Nearest Neighbors (KNN)** | 42.07%            | 6.67%            |
| **Support Vector Regression** | 20.36%            | 21.70%           |
| **Decision Tree Regression**  | 99.90%            | 12.87%           |
| **Random Forest Regression**  | 93.42%            | 57.19%           |

**Observations:**

- Tree-based models (**Decision Tree, Random Forest**) tend to overfit on training data.
- **Regularized regression models (Lasso & Ridge) performed well** in reducing overfitting.
- **SVR and KNN showed varying performance** based on hyperparameter tuning.

---

## 🚀 Installation & Usage

### Prerequisites:

Ensure you have **Python 3.x** installed with required dependencies.

### 🛆 Install Required Libraries:

```bash
pip install pandas numpy matplotlib sklearn
```

## 🔧 Running the Project:
**1. Clone the repository:**
  ```bash
  git clone https://github.com/your-username/cancer-regression.git
  ```
**2. Navigate to the project folder:**
  ```bash
  cd cancer-regression
  ```
**3. Open and run the Jupyter Notebook:**
  ```bash
  jupyter notebook "Cancer_Regression.ipynb"
  ```
## 📌 Key Takeaways:

- **Polynomial Regression** is highly unstable, leading to poor generalization.
- **Lasso and Ridge regression** provide the best balance between bias and variance.
- **Random Forest and Decision Tree models** tend to overfit, requiring pruning or hyperparameter tuning.
- **Feature selection and scaling** significantly impact model performance.

## 🐝 License
- This project is licensed under the **MIT License**.
