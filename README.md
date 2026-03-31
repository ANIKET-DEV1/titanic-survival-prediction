# Titanic Survival Prediction (Machine Learning Project)

## 📌 Problem Statement

The goal of this project is to predict whether a passenger survived the Titanic disaster based on features such as age, gender, ticket class, and fare.

---

## 🧠 Approach

### 1. Data Cleaning

* Handled missing values (Age, Embarked)
* Dropped columns with excessive missing data (e.g., Cabin)
* Converted categorical variables into usable format

---

### 2. Exploratory Data Analysis (EDA)

Performed analysis using **Seaborn** and **Pandas** to understand relationships between features and survival.

Key explorations:

* Survival distribution
* Survival by Gender (Sex / Title)
* Survival by Passenger Class (Pclass)
* Fare vs Survival
* Age group analysis

---

### 3. Feature Engineering

Created meaningful features to improve model performance:

* **Title Extraction** from Name (Mr, Miss, Mrs, Rare)
* **Age Grouping** (Child, Teen, Adult, Old)
* **FamilySize** (SibSp + Parch)
* Converted categorical features into numerical format

---

### 4. Encoding Techniques

Applied different encoding strategies:

* One-Hot Encoding for categorical variables (Title, AgeGroup)
* Label encoding for binary features (Sex)

Later improved preprocessing using:

* **ColumnTransformer**
* Structured encoding pipeline

---

### 5. Model Building

Built classification models using **scikit-learn**:

* Logistic Regression (baseline model)

---

### 6. Model Evaluation

**Accuracy:** ~79–80%

Classification Report Insights:

* Better performance in predicting non-survivors
* Slightly lower recall for survivors (~70%)
* Indicates class imbalance and feature limitations

---

## 🔍 Key Insights

* Gender (Title) is the strongest predictor of survival
* Passenger Class significantly impacts survival
* Higher Fare correlates with higher survival probability
* Combination of features (e.g., Mr + 3rd class) leads to lowest survival

---

## 🛠️ Tools & Libraries Used

* Python
* Pandas
* NumPy
* Seaborn
* Matplotlib
* Scikit-learn

---

## 🚀 Improvements Made

* Added feature engineering (Title, AgeGroup)
* Applied One-Hot Encoding
* Introduced ColumnTransformer for structured preprocessing
* Improved model evaluation using precision, recall, and F1-score

---

## 📈 Future Work

* Try advanced models (Random Forest, etc.)
* Perform hyperparameter tuning
* Improve recall for survivor class
* Build complete ML pipeline
* Deploy model using Flask or API

---

## 📂 Project Structure

```
Titanic-ML-Project/
│
├── data/
├── main.ipynb //Model
├── mainsk.ipynb //Encoding Pracice
├── README.md
```

---

## 🎯 Conclusion

This project demonstrates a complete beginner-to-intermediate machine learning workflow:

* Data Cleaning → EDA → Feature Engineering → Modeling → Evaluation
  
It highlights the importance of data preprocessing and feature engineering in improving model performance.

---
