# Titanic-Survival-Prediction
Predicting passenger survival on the Titanic using machine learning. Includes EDA, feature engineering, and multiple classification models, with Decision Tree achieving 89.6% accuracy on the test set.
# Titanic Survival Prediction

<p align="left">
  <img alt="Python" src="https://img.shields.io/badge/Python-3.x-blue">
  <img alt="Pandas" src="https://img.shields.io/badge/Pandas-Data%20Analysis-informational">
  <img alt="NumPy" src="https://img.shields.io/badge/NumPy-Linear%20Algebra-informational">
  <img alt="Matplotlib" src="https://img.shields.io/badge/Matplotlib-Visualization-informational">
  <img alt="Seaborn" src="https://img.shields.io/badge/Seaborn-Visualization-informational">
  <img alt="scikit-learn" src="https://img.shields.io/badge/scikit--learn-ML%20Models-orange">
  <img alt="License" src="https://img.shields.io/badge/License-MIT-green">
</p>

## 🛠 Tech Stack
- **Language:** Python  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn  
- **Techniques:** EDA, Feature Engineering, Encoding, Age Grouping, Model Training & Evaluation (Logistic Regression, Decision Tree, SVM, KNN)  
- **Environment:** Jupyter Notebook

---

## 📌 Project Overview
A machine learning project to predict passenger survival on the Titanic based on demographics, ticket class, and other features.  
This project is inspired by Kaggle’s classic competition *Titanic: Machine Learning from Disaster*.

---

## 📂 Dataset
- **Source:** [Kaggle – Titanic: Machine Learning from Disaster](https://www.kaggle.com/c/titanic)  
- **Train Set:** `titanic_train.csv` — 891 rows × 12 columns  
- **Test Set:** `titanic_test.csv`  
- **Target:** `Survived` (0 = No, 1 = Yes)  
- **Key Features:** Pclass, Sex, Age, SibSp, Parch, Fare, Embarked  

---

## 🔍 Exploratory Data Analysis (EDA) Insights
- **Females** had a significantly higher survival rate than males.  
- **First-class** passengers had better survival chances compared to second and third class.  
- Survival varied with **embarkation port** (highest from Cherbourg).  
- **Younger passengers** generally had higher survival rates.  
- Large families (high SibSp or Parch) had lower survival chances.

---

## ⚙️ Data Preprocessing
- Dropped non-essential columns: `PassengerId`, `Name`, `Cabin`, `Ticket`.  
- Filled missing values (`Age` with median, `Embarked` with most frequent).  
- Converted `Sex` to binary (male = 1, female = 0).  
- Label-encoded `Embarked`.  
- Created **age group categories**: infant, teen, 20s, 30s, 40s, 50s, elder.

---

## 🤖 Models Trained & Performance
| Model                   | Training Accuracy |
|-------------------------|-------------------|
| Logistic Regression     | 81.9%             |
| Decision Tree Classifier| **94.0%**         |
| Support Vector Machine  | 70.2%             |
| K-Nearest Neighbors     | 81.3%             |

> Decision Tree achieved the highest training accuracy and was used for final test predictions, scoring **89.6%** accuracy.

---

## 📈 Visualizations
- Count plots for categorical features vs. survival  
- Histograms for continuous features  
- Correlation heatmap  
- Confusion matrix for final model predictions

---

