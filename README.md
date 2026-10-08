# SWYNEX Data Science Internship — Task 1

## Data Cleaning and Preparation

### Objective

Select a public dataset, clean missing values, handle data types, and document the assumptions made during data preprocessing.

### Dataset

**Titanic Passenger Dataset**

The dataset contains information about 891 Titanic passengers across 12 columns, including passenger class, age, sex, fare, cabin information, and embarkation port.

### Technologies Used

* Python
* Pandas
* NumPy
* Jupyter Notebook

### Data Cleaning Performed

* Inspected the dataset structure, columns, data types, missing values, and duplicate records.
* Replaced 177 missing `Age` values with the median age of 28.0.
* Replaced 687 missing `Cabin` values with `"Unknown"` because the original cabin information was unavailable.
* Replaced 2 missing `Embarked` values with the most frequent category, `"S"`.
* Checked for duplicate rows; no duplicates were found.
* Verified that the existing data types were appropriate for analysis.
* Checked numerical columns for unusual or invalid values.
* Saved the cleaned dataset as `cleaned_titanic.csv`.

### Assumptions

1. Median imputation was used for missing `Age` values because Age is numerical and the median is less affected by extreme values.
2. Missing Cabin values were represented as `"Unknown"` rather than creating fabricated cabin information.
3. Missing Embarked values were replaced with the mode because Embarked is a categorical variable.
4. Existing data types were retained because they were suitable for analysis and future machine-learning applications.
5. No rows were removed due to missing values to avoid unnecessary data loss.

### Repository Contents

```text
SWYNEX-Task-1/
│
├── task1_data_cleaning.ipynb
├── titanic.csv
├── cleaned_titanic.csv
└── README.md
```

### Outcome

The dataset was successfully cleaned and prepared for further exploratory data analysis and machine-learning tasks.
