# 📊 Adult Dataset Analysis

## 📌 Project Overview

This project focuses on performing **Data Cleaning, Data Preprocessing, Exploratory Data Analysis (EDA), and Data Visualization** using the **Adult Income Dataset (`adult.csv`)**.

The dataset contains information about individuals such as age, education, occupation, workclass, marital status, hours worked per week, and income category.

The main objective of this project is to understand the dataset, handle missing and inconsistent values, perform different data analysis operations, and visualize important patterns using Python.

---

## 📂 Dataset

**Dataset Name:** `adult.csv`

The dataset contains information about individuals and their demographic and employment-related attributes.

### Some important columns include:

* Age
* Workclass
* Education
* Education Number
* Marital Status
* Occupation
* Relationship
* Race
* Sex
* Capital Gain
* Capital Loss
* Hours per Week
* Native Country
* Income

---

## 🛠️ Technologies & Libraries Used

* 🐍 Python
* 🐼 Pandas
* 🔢 NumPy
* 📈 Matplotlib
* 📊 Seaborn
* 📉 Plotly
* ☁️ Google Colab
* 🐙 GitHub

---

## 🔍 Operations Performed

### 1. Importing Required Libraries

Imported Python libraries required for data analysis and visualization.

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import plotly.express as px
```

### 2. Loading the Dataset

Loaded the `adult.csv` dataset using Pandas.

```python
df = pd.read_csv("adult.csv")
```

### 3. Understanding the Dataset

Performed basic dataset exploration using:

* `head()`
* `tail()`
* `shape`
* `columns`
* `info()`
* `describe()`
* `dtypes`

### 4. Identifying Missing Values

Checked for missing values and identified missing values represented using `?`.

```python
df.isnull().sum()
```

The `?` values were also identified and handled during data preprocessing.

### 5. Handling Missing Values

Different approaches were explored for handling missing data.

#### Mean Imputation

Mean values were used for appropriate numerical columns.

```python
df["column"].fillna(df["column"].mean(), inplace=True)
```

#### Mode Imputation

Mode was used for appropriate categorical columns.

```python
df["column"].fillna(df["column"].mode()[0], inplace=True)
```

### 6. Data Cleaning

Performed preprocessing operations such as:

* Identifying missing values
* Handling `?` values
* Checking duplicate records
* Checking data types
* Cleaning inconsistent data
* Handling missing values

### 7. Exploratory Data Analysis

Analyzed different columns to understand:

* Age distribution
* Education distribution
* Workclass distribution
* Occupation distribution
* Income categories
* Working hours
* Relationship between different variables

---

## 📊 Data Visualization

Different visualization techniques were used to understand patterns in the dataset.

### 📈 Line Chart

Used to visualize trends and relationships between numerical variables.

### 📊 Bar Chart

Used to compare categories such as education, occupation, and income.

### 🔵 Count Plot

Used to display the frequency of categorical values.

### 📉 Other Visualizations

The project also explores different charts using:

* Matplotlib
* Seaborn
* Plotly

These visualizations make it easier to identify patterns and relationships within the dataset.

---

## 📌 Key Learning Outcomes

Through this project, I learned how to:

* Load datasets using Pandas
* Explore and understand datasets
* Identify missing values
* Handle missing values using **Mean and Mode**
* Clean real-world datasets
* Perform exploratory data analysis
* Work with categorical and numerical data
* Create different types of visualizations
* Use Matplotlib, Seaborn, and Plotly
* Analyze patterns and relationships in data
* Work with datasets using Google Colab
* Upload and maintain data analysis projects on GitHub

---

## 📁 Project Structure

```text
Adult-Dataset-Analysis/
│
├── adult.csv
├── Adult_Dataset_Analysis.ipynb
└── README.md
```

---

## 🔗 Project Notebook

The complete analysis and Python implementation can be viewed in my Google Colab notebook:

**Google Colab:**
https://colab.research.google.com/drive/1UA6wkGPey13-dyjsYtYQ0p-G0DNyeNDP?usp=sharing

---

## 👩‍💻 Author

**Sandeepa Sandy**

B.Tech – Computer Science and Engineering

---

⭐ If you found this project useful, feel free to explore the repository and the notebook!

