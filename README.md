# AI vs Jobs: Complete Exploratory Data Analysis & Prediction

## Overview

This project explores the impact of Artificial Intelligence on the future job market using the **AI Impact on Jobs 2030** dataset.

The notebook performs:

- Data Loading and Inspection
- Data Cleaning & Validation
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Machine Learning Modeling
- Feature Importance Analysis

The goal is to understand how factors such as automation risk, education level, industry, salary, and experience influence future job growth.

---

## Dataset

Dataset: **AI Impact on Jobs 2030**

The dataset contains information about:

- Job Titles
- Industries
- Countries
- Education Levels
- Years of Experience
- Average Salaries
- Automation Levels
- AI Replacement Risk
- Future Demand Score
- Company Size
- Hiring Trends
- Job Growth Predictions for 2030

---

## Project Workflow

### 1. Data Inspection

Performed basic exploratory checks:

- Dataset Shape
- Summary Statistics
- Data Types
- Missing Values
- Duplicate Records
- Unique Value Counts

---

### 2. Exploratory Data Analysis (EDA)

Several visualizations were created to understand the dataset:

#### Job Market Analysis

- Job Title Distribution
- Industry Distribution
- Country Distribution

#### Workforce Analysis

- Education Level Distribution
- Years of Experience Distribution
- Company Size Distribution

#### Salary Analysis

- Salary Distribution
- Salary by Education Level

#### AI Impact Analysis

- Automation Level Distribution
- AI Replacement Risk vs Future Demand Score
- Hiring Trend Analysis

---

### 3. Feature Engineering

Categorical variables were converted into numerical format using:

```python
LabelEncoder()
```

This enabled machine learning algorithms to process the data.

---

### 4. Machine Learning Model

A **Random Forest Regressor** was trained to predict:

```text
Job_Growth_2030
```

#### Train-Test Split

```python
test_size = 0.2
random_state = 42
```

#### Model

```python
RandomForestRegressor(random_state=42)
```

---

### 5. Model Evaluation

Performance was evaluated using:

- Mean Absolute Error (MAE)
- R² Score

```python
mean_absolute_error()
r2_score()
```

---

### 6. Feature Importance

Feature importance analysis was performed to identify the strongest factors influencing future job growth predictions.

Visualization:

- Top predictive features
- Importance ranking

---

## Libraries Used

```python
pandas
numpy
matplotlib
seaborn
plotly
scikit-learn
```

---

## Key Insights

- AI adoption impacts job demand differently across industries.
- Automation risk varies significantly between job roles.
- Education level influences salary and future opportunities.
- Future demand scores are strongly related to AI replacement risk.
- Certain features contribute more significantly to job growth prediction.

---

## Project Structure

```
├── ai-vs-jobs-complete-exploratory-data-analysis.ipynb
├── README.md
└── dataset
```

---

## Results

The Random Forest model was used to predict future job growth trends and identify the most influential factors affecting employment opportunities in the AI era.

---

## Future Improvements

- Hyperparameter tuning
- Cross-validation
- XGBoost/CatBoost models
- Advanced feature engineering
- Interactive dashboard deployment

---

## Author

Aleesha Nadeem

If you found this project useful, feel free to ⭐ the repository.
