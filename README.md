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
