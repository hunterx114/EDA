# 📊 HR Analytics - Exploratory Data Analysis (EDA)

This project performs an in-depth Exploratory Data Analysis on an HR dataset to identify trends, outliers, and key factors influencing employee attrition.

---

## 🔍 Objective

Understand the HR data using:
- Descriptive statistics
- Visual analysis (histograms, boxplots, pairplots)
- Correlation matrix
- Outlier and pattern detection

Dataset: `HR_comma_sep.csv`

---

## 📁 Dataset Features

| Column                 | Description                                  |
|------------------------|----------------------------------------------|
| satisfaction_level     | Employee satisfaction (0 to 1)               |
| last_evaluation        | Last performance score                       |
| number_project         | Number of projects handled                   |
| average_montly_hours   | Monthly working hours                        |
| time_spend_company     | Years at the company                         |
| Work_accident          | Whether had an accident                      |
| left                   | 1 = Left company, 0 = Still working          |
| promotion_last_5years  | 1 = Promoted, 0 = Not                        |
| department             | Department name                              |
| salary                 | Categorical: low / medium / high             |

---

## 📈 Steps Performed

### 1. Data Loading and Summary
- Checked nulls, data types, shape
- Used `.describe()` to get basic statistics

### 2. Univariate Analysis
- Plotted histograms for numeric columns
- Plotted count plots for categorical columns

### 3. Bivariate Analysis
- Boxplots of numeric columns vs `left`
- Pairplot with `hue='left'`
- Correlation heatmap using Seaborn

### 4. Outlier Detection
- Loop-based boxplots show outliers and median shift
- Insights on overwork, high projects, etc.

### 5. Categorical Encoding
- Converted `salary` and `department` to numeric for ML-readiness

---

## 🧠 Key Insights

- Employees with **low satisfaction** or **extremely high/low project count** tend to leave.
- Long working hours are also related to attrition.
- Employees with **low salary** leave more often.
- Some outliers in `average_montly_hours` and `time_spend_company`.

---

## 💻 Libraries Used

- Python
- Pandas
- NumPy
- Seaborn
- Matplotlib

---

## 📂 Files Included

| File Name              | Description                                 |
|------------------------|---------------------------------------------|
| `EDA IN HR DATASET.ipynb` | Full EDA Jupyter Notebook                  |
| `HR_comma_sep.csv`     | Dataset used                                |
| `README.md`            | This file                                   |

---

## ✅ Status: Task Completed

This project fulfills all the required objectives from the AI & ML Internship **Task 2: Exploratory Data Analysis**.

