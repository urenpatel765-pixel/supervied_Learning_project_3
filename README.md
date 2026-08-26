# 🏦 Banking Risk Prediction using Machine Learning

## 📌 Project Overview

This project uses Machine Learning to predict the risk status of banking customers.

The target variable is **Risk Status**:

- 🟢 `0` = Low Risk
- 🔴 `1` = High Risk

The main goal is to correctly identify **High Risk customers**. Since missing a genuinely High Risk customer can create financial risk for a bank, **Recall and False Negatives** are given special importance.

---

## 🎯 Project Objectives

- 📊 Understand and explore the banking risk dataset.
- 🧹 Preprocess the data for machine learning.
- 🤖 Build classification models for risk prediction.
- ⚖️ Handle class imbalance using different sampling techniques.
- 🌳 Train and compare Decision Tree and Random Forest models.
- 🔧 Tune model hyperparameters using RandomizedSearchCV and GridSearchCV.
- 📈 Evaluate models using multiple performance metrics.
- 🏆 Select the best final model.
- 💼 Explain the results from a business perspective.

---

# 📚 Project Parts

## 🧠 Part A — Conceptual Understanding

This part covers the basic concepts required for the project:

- Logistic Regression
- Classification
- Accuracy
- Precision
- Recall
- F1-Score
- TPR and FPR
- ROC-AUC
- Type-I Error
- Type-II Error
- Imbalanced Data

---

## 🔍 Part B — Data Understanding & Exploration

The dataset is explored before building the models.

The analysis includes:

- 📋 Dataset structure
- 🔢 Data types
- ❓ Missing values
- 📊 Class distribution
- 📈 Data visualization
- 🔎 Understanding relationships between variables

---

## 🧹 Part C — Data Preprocessing & Baseline Model

The dataset is prepared for machine learning using appropriate preprocessing techniques.

The preprocessing includes:

- Missing value handling
- Numerical feature preprocessing
- Categorical feature encoding
- Feature scaling
- Train-test splitting

A baseline classification model is also created for comparison.

---

## ⚖️ Part D — Handling Imbalanced Data

Class imbalance can cause a model to focus mainly on the majority class.

Different techniques are considered to improve identification of the minority class:

- ⬇️ Under-Sampling
- ⬆️ Over-Sampling
- 🔄 SMOTE
- 🔄 ADASYN

The main objective is to improve the model's ability to identify **High Risk customers**.

---

## 🌳 Part E — Decision Tree & Random Forest

Two important tree-based classification models are developed:

### 🌿 Decision Tree

A Decision Tree makes predictions by creating a series of decision rules based on the input features.

### 🌲 Random Forest

Random Forest combines multiple decision trees to produce a stronger and more stable prediction.

Models are evaluated using:

- 🎯 Accuracy
- 🎯 Precision
- 🎯 Recall
- 🎯 F1-Score
- 📈 ROC-AUC
- ❌ False Positives
- ❌ False Negatives

---

# 🔧 Part F — Hyperparameter Tuning

Hyperparameter tuning is performed to improve model performance.

### 🔀 RandomizedSearchCV

RandomizedSearchCV explores a larger parameter space by testing selected random combinations of hyperparameters.

### 🔎 GridSearchCV

GridSearchCV performs a more systematic search over a focused range of parameter values.

### 🔄 Cross-Validation

**5-Fold Stratified Cross-Validation** is used.

The main scoring metric is:

> 🎯 **Recall**

Recall is important because the project focuses on correctly identifying **High Risk customers**.

---

# 📊 Part G — Final Model Evaluation

The tuned and untuned models are compared using the same test dataset.

The evaluation includes:

- 📈 ROC Curves
- 📊 ROC-AUC Comparison
- 🔲 Confusion Matrices
- ❌ False Positive Comparison
- ❌ False Negative Comparison
- 📋 Complete Performance Comparison
- 💼 Business-focused Model Selection

---

# 📝 Part H — Final Report & Conclusion

The final section contains:

- 🏆 Final model
- 📊 Final performance
- 🔧 Best hyperparameters
- 💼 Business interpretation
- ⚠️ Project limitations
- 🚀 Future improvements
- 📝 Final conclusion

---

# 🛠️ Technologies & Libraries

The project is implemented using **Python**.

### 💻 Technologies

- 🐍 Python
- 📓 Jupyter Notebook
- 🤖 Scikit-learn
- ⚖️ Imbalanced-learn

### 📦 Main Libraries

- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn

### 🔧 Important Components

- `StandardScaler`
- `OneHotEncoder`
- `SimpleImputer`
- `KNNImputer`
- `Pipeline`
- `ColumnTransformer`
- `train_test_split`
- `StratifiedKFold`
- `GridSearchCV`
- `RandomizedSearchCV`
- `LogisticRegression`
- `DecisionTreeClassifier`
- `RandomForestClassifier`
- `SVC`
- `KNeighborsClassifier`

### ⚖️ Sampling Techniques

- `RandomUnderSampler`
- `RandomOverSampler`
- `SMOTE`
- `ADASYN`

---

# 📏 Model Evaluation Metrics

### 🎯 Accuracy

Measures the percentage of total predictions that are correct.

### 🎯 Precision

Measures how many customers predicted as High Risk are actually High Risk.

### 🎯 Recall

Measures how many actual High Risk customers are correctly identified.

**Recall is especially important in this project.**

### ⚖️ F1-Score

F1-Score provides a balanced measure of Precision and Recall.

### 📈 ROC-AUC

ROC-AUC measures how well the model distinguishes between Low Risk and High Risk customers.

### ❌ False Positive

A Low Risk customer is incorrectly predicted as High Risk.

### 🚨 False Negative

A High Risk customer is incorrectly predicted as Low Risk.

**False Negatives are especially important because missing a High Risk customer can create financial risk.**

---

# 🔧 Final Hyperparameters

## 🌿 Tuned Decision Tree

```text
criterion = entropy
max_depth = 7
min_samples_leaf = 2
min_samples_split = 15
