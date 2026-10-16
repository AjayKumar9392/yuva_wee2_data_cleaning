# Data Cleaning and Preprocessing | Yuva Internship

## Project Overview

This project focuses on cleaning, validating, and preprocessing
the Online Retail II transaction dataset using Python.

The workflow covers missing-value investigation, duplicate removal,
data standardization, outlier detection, feature engineering, and
demonstrations of encoding and numerical scaling.

## Objectives

- Inspect and understand a real-world retail dataset.
- Identify and remove exact duplicate records.
- Investigate missing values and unusual numerical values.
- Standardize column names and data types.
- Detect outliers using the Interquartile Range (IQR) method.
- Engineer transaction and date-related features.
- Demonstrate categorical encoding and numerical preprocessing.
- Produce a data-quality report and visual output.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Dataset

The project uses the Online Retail II dataset, combining the
2009–2010 and 2010–2011 worksheets.

The dataset contains invoice information, product details,
quantities, prices, dates, customer identifiers, and countries.

The original dataset is not included in this repository.
Obtain it from an authorized source before running the notebook.

## Data Cleaning

The cleaning workflow includes:

1. Combining both source worksheets.
2. Removing exact duplicate rows.
3. Recovering descriptions when a product code has one
   unambiguous description.
4. Investigating unresolved missing values.
5. Standardizing column names and data types.
6. Investigating negative quantities and unusual prices.
7. Detecting statistical outliers using IQR bounds.

## Feature Engineering

The project creates features including:

- Transaction value
- Invoice year
- Invoice month
- Invoice quarter
- Invoice day
- Day of the week
- Invoice hour
- Year-month period
- Transaction type

## Preprocessing Demonstrations

The notebook demonstrates:

- One-hot encoding
- StandardScaler
- MinMaxScaler
- Row-wise normalization

These transformations are demonstrated separately from the
master transaction dataset.

## Results

- 1,067,371 records were initially combined from both worksheets.
- 34,335 exact duplicate rows were removed.
- 1,033,036 records remained after duplicate removal.
- Missing descriptions and customer identifiers were investigated.
- IQR outlier detection was performed on quantity, price,
  and transaction value.
- Nine engineered features were verified.
- A data-quality report, outlier chart, and Word report were generated.

## Project Structure

```text
data/
notebooks/
outputs/
README.md
requirements.txt
.gitignore
