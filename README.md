# synent-task1-titanicdatacleaning-gershom
Cleaning and Preprocessing data to ensure that the data is ready for analysis
# Synent Task 1: Titanic Data Cleaning & Preprocessing

**Author:** Gershom Mosora Nyamongo
**Program:** Synent Technologies - Data Science Internship (Task 1)
**Demo video:** https://youtu.be/dVOYlWf6pUw

## Problem Statement
Raw data is rarely ready for analysis. This project cleans and prepares the Titanic passenger dataset by handling missing values, removing duplicates, converting data types and renaming columns.

## Dataset
I obtained the Titanic dataset from Kaggle: 891 rows and 10 columns (sex, age, siblings/spouses, parents/children, fare, port of embarkation, class, passenger type, alone, survived). Files: Titanic.csv (raw) and Titanic_clean.csv (cleaned).

## Approach
- Inspected the data: age had 177 missing values, embarked had 2, and there were 111 duplicate rows.
- Removed the duplicates first, so they would not affect the values used to fill gaps.
- Filled missing ages with the median age of passengers with the same gender and class, and missing ports with the most common port.
- Removed 8 rows that became identical after filling the ages.
- Converted text columns to the category type.
- Renamed columns (for example sibsp to siblings_spouses) and replaced port codes with full names.

## Results
- Rows: 891 to 772
- Missing values: 179 to 0
- Duplicates: 111 to 0
- The clean data is saved as Titanic_clean.csv.

## Tools
Python, pandas, Jupyter Notebook
