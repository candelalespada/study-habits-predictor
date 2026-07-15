# study-habits-predictor
A machine learning project analyzing whether self-reported study habits and behaviors can predict academic performance, using survey data from CMSC320 students.

## Problem

Understanding which behaviors actually predict academic outcomes could help students and instructors identify at-risk students early and target interventions before it's too late.

## Approach

- Collected survey responses from 188 CMSC320 students, covering study habits (hours studied, sleep, lecture attendance, reading completion, screen time, etc.) alongside actual exam scores
- Cleaned data: removed irrelevant columns (timestamps, index, unreliable responses), computed exam percentage
- One-hot encoded categorical variables, retained numeric variables in original form
- Modeled three separate prediction problems:
  1. **Pass/Fail** — binary classification
  2. **Letter Grade** — multiclass classification (A–F)
  3. **Exact Exam Score** — regression
- Applied and compared three algorithms: Logistic Regression, Decision Tree, and K-Nearest Neighbors (KNN)

## Tech Stack

- Python
- scikit-learn
- Pandas
- NumPy
- Data Visualization (Matplotlib)
