# Portugese-bank-marketing
# 📊 Portuguese Bank Marketing Prediction

This project focuses on analyzing and predicting whether a client will **subscribe to a term deposit** using the **Bank Marketing Dataset** provided by a Portuguese banking institution. The complete workflow includes data preprocessing, exploratory data analysis (EDA), machine learning model building, and evaluation.

---

## 📝 Problem Statement

The bank conducted direct marketing campaigns via phone calls to promote term deposit subscriptions. The goal is to build a classification model that predicts whether a client will subscribe based on historical campaign data.

---

## 📂 Dataset Overview

- **Source**: UCI Machine Learning Repository  
- **Link**: [Bank Marketing Dataset](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing)  
- **Instances**: 41,188  
- **Features**: 20  
- **Target Variable**: `y` — whether the client subscribed to a term deposit (`yes`/`no`)

### 📌 Key Features

| Feature      | Description                                 |
|--------------|---------------------------------------------|
| age          | Client's age                                |
| job          | Type of job                                 |
| marital      | Marital status                              |
| education    | Education level                             |
| default      | Has credit in default?                      |
| balance      | Average yearly balance (in euros)           |
| housing      | Has a housing loan?                         |
| loan         | Has a personal loan?                        |
| contact      | Contact communication type                  |
| day/month    | Last contact date                           |
| duration     | Last contact duration (in seconds)          |
| campaign     | Number of contacts in this campaign         |
| pdays        | Days since last contact (-1 = never)        |
| previous     | Number of previous contacts                 |
| poutcome     | Outcome of the previous campaign            |
| y            | 💡 Target variable (yes = subscribed)       |

---

## 🔧 Technologies Used

- Python 3.x
- pandas, NumPy
- matplotlib, seaborn
- scikit-learn
- XGBoost
- Jupyter Notebook

---

## 📊 Exploratory Data Analysis (EDA)

- Target class distribution
- Job and education vs. subscription rate
- Balance, duration, and campaign effectiveness
- Correlation heatmaps and boxplots
- Time-based patterns using month and day

---

## 🔄 Preprocessing

- Handled `unknown` values in categorical features
- Applied Label Encoding and One-Hot Encoding
- Removed outliers and duplicate rows (if any)
- Scaled numerical features using `StandardScaler`
- Handled class imbalance with resampling (optional)
- Train-test split (typically 80:20)

---

## 🤖 Models Applied

| Model               | Description                  |
|--------------------|------------------------------|
| Logistic Regression| Baseline binary classifier   |
| Decision Tree       | Tree-based modeling          |
| Random Forest       | Ensemble model               |
| XGBoost             | Gradient boosting classifier |
| Support Vector Machine (SVM) | Margin-based model |

---

## 📈 Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC
- Confusion Matrix

### ✅ Sample Results

| Model            | Accuracy | ROC-AUC |
|------------------|----------|---------|
| Logistic Regression | 89.3% | 0.92    |
| Random Forest       | 91.7% | 0.94    |
| XGBoost             | 93.1% | 0.95    |

> Note: Metrics may vary based on preprocessing and tuning.

---

## 🧪 How to Run the Project

1. Clone the repository:
```bash
git clone https://github.com/yourusername/portuguese-bank-marketing.git
cd portuguese-bank-marketing
