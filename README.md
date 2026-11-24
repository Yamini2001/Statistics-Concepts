# Pandas Data Manipulation Practice

## Overview

This repository contains hands-on practice of Python libraries **Pandas** and **NumPy**. It focuses on performing data manipulation, data cleaning, filtering, and statistical analysis using a sample Employee Dataset.

The objective is to understand how to work with structured data using Pandas DataFrames and perform basic data analysis operations.

## Technologies Used

- Python
- Pandas
- NumPy
- Jupyter Notebook

## Concepts Covered

### 1. Importing Libraries

Importing Pandas and NumPy for data manipulation and numerical operations.

```python
import pandas as pd
import numpy as np
```

### 2. Creating a DataFrame

Creating an Employee Dataset using Pandas DataFrame.

The dataset contains:
- Employee Name
- Age
- Salary
- Department

### 3. Renaming Columns

Using the `rename()` function to modify DataFrame column names.

```python
df.rename(columns={'Name': 'Employee_Name'})
```

### 4. Handling Missing Values

Handling missing values using Pandas functions such as:

- `fillna()` – Replace missing values.
- `mode()` – Find the most frequently occurring value.

```python
df['Department'].fillna(
    df['Department'].mode()[0],
    inplace=True
)
```

### 5. Filtering Data

Filtering employees based on specific conditions.

**Employees belonging to the IT department:**

```python
df[df['Department'] == 'IT']
```

**Employees earning more than 60000:**

```python
df[df['Salary'] > 60000]
```

### 6. Statistical Operations

Calculating the average salary of employees.

```python
df['Salary'].mean()
```

### 7. GroupBy Operations

Grouping employees based on their department and calculating the average salary.

```python
df.groupby('Department')['Salary'].mean()
```

## Installation and Setup

### Step 1: Clone the Repository

```bash
git clone <your-github-repository-url>
```

### Step 2: Navigate to the Project

```bash
cd pandas-data-manipulation-practice
```

### Step 3: Install Dependencies

```bash
pip install pandas numpy jupyter
```

### Step 4: Launch Jupyter Notebook

```bash
jupyter notebook
```

Open the notebook inside the `notebooks` directory and execute the cells sequentially.

## Learning Objectives

- Understand Pandas DataFrame operations.
- Perform basic data cleaning.
- Handle missing values.
- Apply conditional filtering.
- Perform statistical calculations.
- Understand grouping and aggregation.
- Develop practical data analysis skills.

## Future Enhancements

- Explore advanced Pandas operations.
- Perform data visualization.
- Work with CSV and Excel datasets.
- Implement real-world ETL operations.
- Perform exploratory data analysis (EDA).



GitHub: <your-github-profile-url>

---

*This repository is part of my practical learning journey in Statistics, Python, and Data Analytics.*
