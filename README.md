# university-practical-training

# Part1: Task's DATA HANDLING

## Task1: Basic Statistics Using Python

This project is a simple Python assignment that takes a list of numbers from the user and performs basic statistical operations.

### About the Task

The program allows the user to enter numbers separated by spaces or commas, then stores and processes the numbers using Python data structures.

### Features

* Store numbers in a list
* Count the frequency of each number using a dictionary
* Calculate the sum
* Calculate the average
* Find the maximum value
* Find the minimum value
* Sort the numbers
* Display the most frequent number
* Allow the user to choose a specific statistical operation

### Example Input

```text
5 10 5 20 10
```

### Example Output

```text
Sum: 50.0
Average: 10.00
Maximum value: 20.0
Minimum value: 5.0
Frequency dictionary: {5.0: 2, 10.0: 2, 20.0: 1}
```

### Tools Used

* Python
* Google Colab / Jupyter Notebook

### Purpose

The purpose of this task is to practice basic Python programming concepts such as lists, dictionaries, loops, functions, input handling, and simple statistics.

---

## Task2: Titanic Data Cleaning and Analysis Using Python

This project is a Python data analysis assignment that uses the Titanic dataset to practice data cleaning, grouping, merging, pivot tables, feature engineering, and outlier handling using Pandas.

### About the Task

The program loads the Titanic dataset from an online CSV file, cleans missing data, standardizes formats, performs statistical grouping, creates a pivot table, engineers a new travel group feature, and handles Fare outliers using the IQR method.

### Features

* Load the Titanic dataset from a CSV URL
* Store and process data using a Pandas DataFrame
* Handle missing values in the Age column using the median
* Fill missing Embarked values using the mode
* Drop the Cabin column because it contains many missing values
* Standardize passenger names using title case
* Group passengers by ticket class
* Calculate the average Fare for each class
* Count the number of passengers in each class
* Create a secondary DataFrame for class descriptions
* Merge grouped results with class descriptions
* Create a pivot table showing mean Fare by Embarked and Sex
* Create a TravelGroup feature based on SibSp and Parch
* Handle Fare outliers using the IQR method
* Store final summary statistics in a dictionary

### Dataset Used

```text
https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv
```

### Main Columns Used

* PassengerId
* Name
* Sex
* Age
* Pclass
* Fare
* SibSp
* Parch
* Embarked

### Example Operations

```text
Age missing values are replaced with the median age.
Embarked missing values are replaced with the most frequent value.
Cabin column is removed.
Passengers are grouped by Pclass.
A pivot table is created using Embarked and Sex.
TravelGroup is created from SibSp + Parch + 1.
Fare outliers are handled using the IQR method.
```

### Tools Used

* Python
* Pandas
* Google Colab / Jupyter Notebook

### Purpose

The purpose of this task is to practice real-world data handling and data analysis skills using Python. It focuses on cleaning messy data, summarizing information, creating useful features, and preparing data for deeper analysis or machine learning tasks.

---

## 🧹 Task3: Titanic Dataset Cleaning and Enhancement Using Pandas

![Python](https://img.shields.io/badge/Python-Data%20Cleaning-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green)
![Google Colab](https://img.shields.io/badge/Google%20Colab-Notebook-orange)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

This project focuses on cleaning and enhancing the Titanic dataset using Python and Pandas in Google Colab.  
The goal of this task is to prepare messy real-world data for data science, visualization, reporting, and AI modeling tasks.

### 📌 About the Task

In this task, the Titanic dataset is loaded, inspected, cleaned, enhanced, and prepared for analysis.  
The project handles common data quality issues such as missing values, duplicate rows, inconsistent text formats, and outliers.

The dataset is improved by creating new useful features such as `FamilySize`, `TravelGroup`, and `AgeGroup`.

### 🎯 Main Objectives

* Load the Titanic dataset using Pandas
* Inspect dataset structure, columns, data types, and summary statistics
* Detect missing values in all columns
* Handle missing data using suitable imputation techniques
* Remove duplicate rows to ensure data integrity
* Standardize text formats for consistency
* Engineer new features from existing columns
* Detect and handle Fare outliers using the IQR method
* Display the final cleaned and enhanced dataset
* Document all cleaning steps for reproducibility

### 🧾 Dataset Used

```text
https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv
```

### 🧼 Data Cleaning Steps

```text
1. Loaded the Titanic dataset from a CSV URL.
2. Checked the dataset shape, column names, data types, and missing values.
3. Filled missing Age values using the median age.
4. Filled missing Embarked values using the most frequent value.
5. Dropped the Cabin column because it had many missing values.
6. Checked and removed duplicate rows.
7. Standardized Name values using title case.
8. Standardized Sex values by converting them to lowercase.
9. Standardized Embarked values by converting them to uppercase.
```

### 🛠️ Feature Engineering

New columns were created to make the dataset more useful for analysis:

| New Feature | Description |
|---|---|
| `FamilySize` | Total number of people traveling together, calculated using `SibSp + Parch + 1` |
| `TravelGroup` | Classifies passengers as `Solo`, `Small`, or `Large` based on family size |
| `AgeGroup` | Classifies passengers into age categories: `Child`, `Teen`, `Adult`, and `Senior` |
| `OriginalFare` | Stores the original Fare values before outlier handling |
| `Fare_Capped` | Stores Fare values after handling outliers using the IQR method |

### 📊 Outlier Handling Method

Fare outliers were handled using the **IQR method**.

```text
Q1 = 7.9104
Q3 = 31.0
IQR = 23.0896
Lower Bound = -26.724
Upper Bound = 65.6344
```

Values above the upper bound were capped to the maximum acceptable value.  
This helped reduce the effect of extreme Fare values on future analysis or modeling.

### ✅ Final Cleaning Summary

| Item | Result |
|---|---:|
| Rows before cleaning | 891 |
| Rows after cleaning | 891 |
| Duplicated rows before cleaning | 0 |
| Median Age used | 28.0 |
| Mode Embarked used | S |
| Fare outliers before handling | 116 |
| Fare outliers after handling | 0 |
| Mean capped Fare | 24.05 |
| Maximum Family Size | 11 |

### 📌 Final Output

The final dataset became cleaner, more consistent, and more suitable for:

* Data visualization
* Statistical analysis
* Reporting
* Machine learning
* AI modeling workflows

### Tools Used

* Python
* Pandas
* Google Colab / Jupyter Notebook

### Purpose

The purpose of this task is to practice real-world data preparation skills.  
Messy datasets are common in data science and AI projects, and cleaning them properly is essential for producing accurate, reliable, and meaningful results.