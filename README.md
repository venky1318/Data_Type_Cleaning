# Task 24 — Data Type Cleaning Using Pandas

## Project Overview

This project demonstrates how to identify incorrect data types in a dataset and convert columns into appropriate data types using Python and Pandas.

A sample employee dataset is used to demonstrate conversions involving integer, floating-point, categorical, and datetime data types.

## Objectives

- Inspect original data types using `dtypes` and `info()`.
- Convert age from string to integer.
- Convert salary from currency-formatted text to numerical values.
- Convert performance scores into floating-point values.
- Convert joining dates into datetime format.
- Convert department into a categorical data type.
- Compare original and corrected data types.
- Validate the conversions.

## Technologies Used

- Python
- Pandas
- NumPy
- Google Colab
- Jupyter Notebook

## Dataset Description

The project uses a manually created employee dataset containing 10 fictional records and seven columns:

- employee_id
- employee_name
- age
- salary
- department
- joining_date
- performance_score

The original dataset is loaded with string data types to demonstrate the conversion process.

## Data Type Conversions

| Column | Original Type | Corrected Type |
|---|---|---|
| employee_id | string | string |
| employee_name | string | string |
| age | string | int64 |
| salary | string | int64 |
| department | string | category |
| joining_date | string | datetime64[ns] |
| performance_score | string | float64 |

## Functions Used

- `df.dtypes` — inspects column data types.
- `df.info()` — displays dataset information.
- `astype()` — converts columns into specified data types.
- `pd.to_numeric()` — converts values into numerical types.
- `pd.to_datetime()` — converts values into datetime format.
- `to_csv()` — exports the cleaned dataset.

## Project Files

- `Task_24_Data_Type_Cleaning.ipynb` — Google Colab notebook.
- `employee_data_raw.csv` — Original dataset.
- `employee_data_cleaned.csv` — Corrected dataset.
- `data_type_comparison.csv` — Original and corrected data type comparison.
- `requirements.txt` — Required libraries.
- `README.md` — Project documentation.
- `project_report.pdf` — Formal project report.
- `screenshots/` — Execution evidence.

## Key Findings

The original dataset is loaded with all columns represented as strings. The cleaning process converts age, salary, performance score, joining date, and department into suitable data types while retaining employee IDs and names as strings.

The conversions are verified using Pandas data type inspection and validation checks.

## Conclusion

This project demonstrates how correct data types improve data consistency and make numerical calculations, date operations, and categorical analysis possible.
