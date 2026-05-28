# Employee Churn Prediction using Machine Learning

## Project Overview
This project builds a machine learning model to predict employee attrition — 
identifying which employees are likely to leave an organization. 
Employee churn is a critical HR challenge, and predicting it early allows 
companies to take proactive retention measures.

This project is directly relevant to HR-tech companies like ADP that manage 
workforce data at scale.

---

## Dataset
- Source: Kaggle — HR Analytics Dataset
- Records: 14,999 employees
- Features: 10 columns including satisfaction level, number of projects,
  average monthly hours, salary, and department
- Target Variable: `left` (1 = Employee Left, 0 = Employee Stayed)

---

## Problem Statement
Given historical HR data, predict whether an employee will leave the company
based on features like satisfaction level, workload, salary, and department.

---

## Tech Stack
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Google Colab / VS Code

---

## Project Structure

-employee-churn-prediction/
-│
-├── HR_comma_sep.csv          # Dataset
-├── employee_churn.ipynb      # Main notebook
-└── README.md                 # Project documentation

---

## Steps Followed

### 1. Data Loading and Exploration
- Loaded dataset using Pandas
- Explored shape, data types, and basic statistics
- Checked class distribution of target variable

### 2. Exploratory Data Analysis
- Identified satisfaction level as the strongest predictor of churn
- Found that employees with low satisfaction and high monthly hours
  had significantly higher churn rates
- Analyzed churn rate by department and salary level

### 3. Data Preprocessing
- Checked and confirmed no missing values
- Encoded categorical variables (Department, salary) using One-Hot Encoding
- Split data into 80% training and 20% testing sets

### 4. Model Training
- Chose Logistic Regression for its interpretability and suitability
  for binary classification problems
- Trained model on 11,999 records

### 5. Model Evaluation
- Achieved 78.23% accuracy on unseen test data
- Evaluated using confusion matrix and classification report
- Analyzed precision, recall, and F1-score for both classes

---

## Results

| Metric | Score |
|--------|-------|
| Accuracy | 78.23% |
| Model | Logistic Regression |
| Train/Test Split | 80/20 |

---

## Key Insights
- Satisfaction level is the strongest predictor of employee churn
- Employees working more than 250 hours per month show higher churn rates
- Low salary employees have significantly higher attrition
- Employees who worked on 6-7 projects showed higher tendency to leave

---

## Future Improvements
- Try ensemble models like Random Forest and XGBoost for better accuracy
- Handle class imbalance using SMOTE oversampling technique
- Build an interactive dashboard using Streamlit
- Deploy model as a REST API using Flask

---

## How to Run

1. Clone this repository
```bash
git clone https://github.com/yourusername/employee-churn-prediction
```

2. Install required libraries
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

3. Open the notebook
```bash
jupyter notebook employee_churn.ipynb
```

Or simply open in Google Colab directly.

---

## Author
**Your Name**
- LinkedIn: https://www.linkedin.com/in/dhruvesh-singh-om
- GitHub: https://github.com/DhruveshOm

---

## Acknowledgements
- Dataset sourced from Kaggle HR Analytics Dataset
- Inspired by real-world HR challenges in workforce retention
