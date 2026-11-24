Pandas Data Manipulation Practice
This repository contains hands-on Python practice using Pandas and
NumPy. The notebook works with a small employee dataset and
demonstrates common DataFrame operations used during data cleaning and
exploratory data analysis.
Notebook
  File                                          Description
  employee-data-cleaning.ipynb   Creates an employee DataFrame and
demonstrates column renaming,
missing-value handling, filtering,
aggregation, and grouping.
Concepts Covered
1. Importing libraries --- use Pandas and NumPy.
2. Creating a DataFrame --- build an employee dataset with Name,
   Age, Salary, and Department columns.
3. Renaming columns --- use DataFrame.rename() to change column
   names.
4. Handling missing values --- use fillna() and mode() to fill
   missing department values.
5. Filtering rows --- select employees by department or salary
   condition.
6. Aggregation --- calculate the average salary with mean().
7. Grouping data --- calculate average salary by department with
   groupby().
Dataset
The notebook creates a sample employee dataset with six records. It
includes employee names, ages, salaries, and departments. Some fields
are initially missing so that missing-value handling can be practised.
Requirements
- Python 3
- Pandas
- NumPy
- Jupyter Notebook or JupyterLab
Install the dependencies:
pip install pandas numpy jupyter
How to Run
1. Clone or download this repository.
2. Open a terminal in the repository directory.
3. Start Jupyter:
   jupyter notebook
4. Open employee-data-cleaning-and-analysis.ipynb.
5. Run the notebook cells in order.
Example Operations
# Employees in the IT department
print(df[df["Department"] == "IT"])

# Employees earning more than 60,000
print(df[df["Salary"] > 60000])

# Overall average salary
print(df["Salary"].mean())

# Average salary by department
print(df.groupby("Department")["Salary"].mean())
Learning Objective
Practise essential Pandas DataFrame operations on a small,
understandable dataset and build a foundation for data cleaning and
analysis workflows.
Note
The notebook is a learning exercise using sample data. Review and run
all cells before relying on saved outputs. In particular, ensure that
the missing-value handling code matches the displayed results, and
display filtered and grouped results explicitly.
