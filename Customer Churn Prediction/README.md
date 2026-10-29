# Customer Churn Prediction Using Feature Engineering

## 📌 Project Overview

Customer churn prediction helps businesses identify customers who are likely to discontinue their services. This project uses the **Telco Customer Churn dataset** to analyze customer behavior and build machine learning models that predict whether a customer will leave the company.

The project focuses on data preprocessing, feature engineering, Logistic Regression, and feature selection to evaluate how different approaches affect model performance.

## 🎯 Objectives

- Analyze customer characteristics and churn patterns.
- Clean and preprocess customer data.
- Engineer meaningful features to improve predictive performance.
- Build a baseline Logistic Regression model.
- Compare baseline and feature-engineered models.
- Evaluate model performance using classification metrics.

## 🛠️ Technologies Used

- **Programming Language:** Python
- **Libraries:** Pandas, NumPy, Scikit-learn
- **Visualization:** Matplotlib, Seaborn
- **Machine Learning:** Logistic Regression, Random Forest
- **Techniques:** Feature Engineering, Feature Selection, Data Preprocessing, Model Evaluation

## 📂 Dataset

The project uses the **Telco Customer Churn dataset**, which contains customer information related to demographics, subscribed services, account details, billing, and churn status.

The target variable is `Churn`, which indicates whether a customer has left the service.

## ⚙️ Project Workflow

### 1. Data Cleaning and Preprocessing
- Converted `TotalCharges` into a numeric format.
- Handled missing values using median imputation.
- Encoded the target variable into a binary format.
- Prepared numerical and categorical features for machine learning.

### 2. Exploratory Data Analysis
- Examined customer attributes and churn patterns.
- Analyzed the relationship between customer characteristics and churn.
- Identified potential features useful for prediction.

### 3. Feature Engineering
Created additional features to capture customer behavior more effectively:
- **Tenure Groups:** Grouped customers based on their tenure.
- **Service Count:** Counted additional services subscribed to by customers.
- **Monthly Charge Ratio:** Derived a feature based on monthly charges.
- **Service Categories:** Simplified selected categories representing unavailable services.

### 4. Model Development
- Developed a baseline Logistic Regression model.
- Used Scikit-learn pipelines for preprocessing and model training.
- Applied `StandardScaler` to numerical features.
- Used `OneHotEncoder` for categorical features.
- Compared model performance before and after feature engineering.

### 5. Feature Selection
- Used Random Forest-based feature importance.
- Applied feature selection to identify relevant predictors.
- Evaluated the effect of selecting features on classification performance.

### 6. Model Evaluation
Evaluated the models using:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

## 📊 Results

The initial model comparison reported the following results:

| Model | Accuracy | Churn-Class F1-Score |
|---|---:|---:|
| Baseline Logistic Regression | 81% | 0.59 |
| Feature-Engineered Logistic Regression | 82% | 0.61 |

Feature engineering showed a small improvement in the initial model comparison. Additional feature-selection experiments were also conducted to study their impact on model performance.

*Note: Results may vary depending on the preprocessing steps, selected features, and train-test split.*

## 💡 Key Learnings

- Importance of cleaning and preprocessing real-world customer data.
- How feature engineering can capture additional customer behavior patterns.
- How Scikit-learn pipelines combine preprocessing and model training.
- How feature selection influences classification performance.
- Why accuracy and F1-score should be evaluated together for churn prediction.

## 🚀 Future Improvements

- Experiment with additional classification algorithms.
- Perform hyperparameter tuning.
- Address class imbalance if required.
- Use cross-validation for more robust evaluation.
- Develop a dashboard to visualize churn patterns and model predictions.

## 👩‍💻 Author

**Nandini Gupta**

- GitHub: [nandini17404](https://github.com/nandini17404)
- LinkedIn: [Nandini Gupta](https://www.linkedin.com/in/nandini-gupta-976aab275/)

---

⭐ If you find this project useful, consider giving the repository a star.
