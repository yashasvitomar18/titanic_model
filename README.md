# 🚢 Titanic Survival Prediction using Machine Learning

## 📌 Project Overview

This project predicts whether a passenger survived the Titanic disaster using various Machine Learning classification algorithms. The dataset is preprocessed, cleaned, encoded, scaled, and used to train multiple classification models for survival prediction.

---

## 🎯 Objective

The main goal of this project is to build and compare different Machine Learning classification algorithms to predict passenger survival on the Titanic dataset.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Jupyter Notebook

---

## 📂 Dataset

The Titanic dataset is loaded directly from Seaborn.

```python
import seaborn as sns

df = sns.load_dataset('titanic')
```

### Features Used

- Pclass
- Sex
- Age
- SibSp
- Parch
- Fare
- Embarked
- Alone

### Target Variable

```python
survived
```

---

## 🔄 Data Preprocessing

### 1. Data Cleaning

Removed unnecessary columns:

```python
deck
adult_male
embark_town
class
who
alive
```

### 2. Handling Missing Values

- Missing values in Age were filled using Mean Imputation.
- Rows with missing values in Embarked were removed.

### 3. Label Encoding

Categorical features encoded:

```python
sex
embarked
```

### 4. Data Type Conversion

Converted features into integer format for model training.

---

## 📊 Train-Test Split

```python
train_test_split(
    X,
    y,
    test_size=0.2,
    random_state=42
)
```

- Training Data: 80%
- Testing Data: 20%

---

## 📈 Feature Scaling

StandardScaler was used for feature normalization.

```python
from sklearn.preprocessing import StandardScaler

scaler = StandardScaler()
```

---

## 🤖 Machine Learning Models Used

### 1. Logistic Regression

```python
from sklearn.linear_model import LogisticRegression
```

### 2. K-Nearest Neighbors (KNN)

```python
from sklearn.neighbors import KNeighborsClassifier
```

### 3. Gaussian Naive Bayes

```python
from sklearn.naive_bayes import GaussianNB
```

### 4. Decision Tree Classifier

```python
from sklearn.tree import DecisionTreeClassifier
```

---

## 📋 Evaluation Metrics

Models were evaluated using:

- Accuracy Score
- Confusion Matrix
- Classification Report

```python
from sklearn.metrics import (
    accuracy_score,
    confusion_matrix,
    classification_report
)
```

---

## 🚀 Project Workflow

```text
Load Dataset
      ↓
Data Cleaning
      ↓
Handle Missing Values
      ↓
Label Encoding
      ↓
Train-Test Split
      ↓
Feature Scaling
      ↓
Model Training
      ↓
Prediction
      ↓
Evaluation
```

---

## 📚 Concepts Practiced

- Data Cleaning
- Missing Value Treatment
- Label Encoding
- Feature Scaling
- Classification Algorithms
- Model Evaluation
- Confusion Matrix
- Performance Metrics

---

## 🔮 Future Improvements

- Hyperparameter Tuning
- Cross Validation
- Random Forest Classifier
- XGBoost Classifier
- Feature Selection
- Streamlit Deployment

---

## 👩‍💻 Author

**Aradhya**

B.Tech Electronics Engineering  
Madhav Institute of Technology & Science (MITS), Gwalior

### Skills

- Python
- SQL
- Pandas
- NumPy
- Machine Learning
- Data Analysis

