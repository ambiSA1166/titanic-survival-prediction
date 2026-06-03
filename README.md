# Titanic: Machine Learning from Disaster

## Project Overview

This project focuses on the classic Titanic dataset to predict passenger survival using machine learning techniques.

The objective was to develop a predictive model while demonstrating proficiency in the complete data science workflow, including:

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Model Training
- Model Validation

---

## Dataset

The dataset comes from the Kaggle competition:

**Titanic: Machine Learning from Disaster**

The goal is to predict whether a passenger survived the Titanic shipwreck based on passenger information such as age, gender, ticket class, and family relationships.

---

## Technical Methodology

### 1. Data Preprocessing

Missing values were handled using appropriate statistical techniques:

- **Age** → Median Imputation
- **Fare** → Median Imputation
- **Embarked** → Mode Imputation

### 2. Feature Engineering

Several new features were created to improve model performance:

#### Title Feature

Extracted passenger titles from names (Mr, Mrs, Miss, etc.) to capture social status.

#### FamilySize Feature

Calculated the total family members aboard:

```python
FamilySize = SibSp + Parch + 1
```

#### IsAlone Feature

Created a binary feature indicating whether a passenger was traveling alone.

---

## Models Used

Three classification algorithms were trained and evaluated:

1. Logistic Regression
2. Decision Tree Classifier
3. Random Forest Classifier

---

## Model Validation

To ensure reliable performance and reduce overfitting, **5-Fold Cross Validation** was used during model evaluation.

This approach helps assess how well the model generalizes to unseen data.

---

## Performance Summary

| Model | Kaggle Public Score |
|---------|---------|
| Logistic Regression | 0.77511 |
| Random Forest Classifier | 0.77033 |
| Decision Tree Classifier | 0.74641 |

### Best Performing Model

**Logistic Regression** achieved the highest Kaggle public leaderboard score.

---

## Tools & Libraries

### Programming Language

- Python

### Data Manipulation

- Pandas
- NumPy

### Data Visualization

- Matplotlib
- Seaborn

### Machine Learning

- Scikit-Learn

---

## Repository Structure

```text
├── Model Building.ipynb
├── submission_logistic_regression.csv
├── README.md
```

### Files Description

#### Model Building.ipynb

Contains the complete machine learning workflow:

- Data Loading
- Data Cleaning
- Exploratory Data Analysis
- Feature Engineering
- Model Training
- Cross Validation
- Prediction Generation

#### submission_logistic_regression.csv

Final prediction file submitted to Kaggle using the Logistic Regression model.

---

## Key Learnings

Through this project, I gained practical experience in:

- Data preprocessing techniques
- Handling missing values
- Feature engineering
- Classification algorithms
- Cross-validation
- Model evaluation
- Kaggle competition workflow

---

## Author

Ambika Gupta

Aspiring Data Scientist | Machine Learning Enthusiast
