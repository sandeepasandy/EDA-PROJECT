📊 Adult Dataset - Exploratory Data Analysis

## 📌 Project Overview

This project focuses on performing **Exploratory Data Analysis (EDA), Data Cleaning, Data Preprocessing, and Data Visualization** on the **Adult Income Dataset (`adult.csv`)** using Python.

Along with traditional Python libraries, this project also explores several **automated EDA and visualization tools** to understand the dataset more efficiently and identify patterns, relationships, missing values, duplicate records, and outliers.

The project was developed and executed using **Google Colab**.

---

## 📂 Dataset

### Adult Income Dataset

The dataset contains information about individuals based on demographic, educational, employment, and financial attributes.

### Dataset Statistics

- **Number of Records:** 32,561
- **Number of Variables:** 15
- **Numerical Variables:** 6
- **Categorical Variables:** 9
- **Target Variable:** Income

---

## 🛠️ Tools & Technologies Used

### Programming Language
- Python 🐍

### Data Analysis
- Pandas
- NumPy

### Data Visualization
- Matplotlib
- Seaborn
- Plotly

### Automated EDA Tools
- D-Tale
- YData Profiling
- AutoViz
- Sweetviz

### Development Environment
- Google Colab
- GitHub

---

## 🔍 Operations Performed

### 1. Data Loading

Loaded the `adult.csv` dataset using Pandas.

```python
import pandas as pd

data = pd.read_csv("adult.csv")
2. Data Exploration

Performed basic dataset exploration using:

head()
tail()
shape
columns
info()
describe()
Data types
Unique values
Value counts
3. Data Cleaning

Performed different data cleaning operations including:

Identifying missing values
Detecting missing values represented by ?
Checking duplicate records
Understanding data types
Handling missing values
Checking inconsistent data
4. Missing Value Handling

Different approaches were explored for handling missing values.

Mean Imputation

Used the mean to fill missing numerical values where appropriate.

data["column"].fillna(data["column"].mean(), inplace=True)
Mode Imputation

Used the mode to fill missing categorical values.

data["column"].fillna(data["column"].mode()[0], inplace=True)
📊 Exploratory Data Analysis

EDA was performed to understand the structure and characteristics of the dataset.

The analysis included:

Distribution of numerical variables
Frequency of categorical variables
Income distribution
Education analysis
Age analysis
Workclass analysis
Occupation analysis
Working hours analysis
Relationships between variables
Outlier identification
Correlation analysis
📈 Data Visualization

Different visualization libraries were used to understand the dataset.

Matplotlib

Created basic charts such as:

Line charts
Bar charts
Histograms
Scatter plots
Seaborn

Created statistical visualizations such as:

Count plots
Bar plots
Histograms
Box plots
Heatmaps
Plotly

Used Plotly for interactive visualizations.

⚡ Automated EDA Tools

One of the main features of this project is the use of multiple automated EDA tools.

🔹 1. D-Tale

D-Tale was used to interactively explore the Pandas DataFrame.

It helps with:

Dataset exploration
Filtering
Sorting
Statistical analysis
Visualization
Data inspection
🔹 2. YData Profiling

YData Profiling was used to automatically generate a detailed Adult Dataset Report.

The report provides information about:

Dataset overview
Variables
Variable types
Missing values
Duplicate rows
Correlations
Sample data
Data quality alerts
from ydata_profiling import ProfileReport

profile = ProfileReport(
    data,
    title="Adult Dataset Report"
)

profile.to_notebook_iframe()
🔹 3. AutoViz

AutoViz was used to automatically generate visualizations from the dataset.

The analysis included the Income variable as the dependent variable and generated multiple visualizations automatically.

AutoViz generated 21 scatter plots during the analysis.

It was also useful for identifying:

Relationships between variables
Outliers
Distributions
Categorical relationships
Potential patterns in the dataset
🔹 4. Sweetviz

Sweetviz was used to generate an automated EDA report.

import sweetviz as sv

report = sv.analyze(data)

report.show_html("sweetviz_report.html")

The generated report provides an interactive overview of the dataset and helps compare and understand different variables.

📌 Key Areas Analyzed

The project explores:

👤 Age
🎓 Education
💼 Workclass
🧑‍💼 Occupation
💰 Income
💍 Marital Status
👨‍👩‍👧 Relationship
🌎 Native Country
⏰ Hours per Week
💵 Capital Gain
💵 Capital Loss
💡 Key Learning Outcomes

Through this project, I learned how to:

Work with real-world datasets
Load and explore CSV files using Pandas
Perform data cleaning and preprocessing
Handle missing values using Mean and Mode
Identify duplicate records
Analyze numerical and categorical variables
Create different types of visualizations
Use Matplotlib, Seaborn and Plotly
Perform automated EDA
Use D-Tale for interactive data exploration
Generate reports using YData Profiling
Automatically generate visualizations using AutoViz
Generate automated EDA reports using Sweetviz
Understand outliers and correlations
Perform exploratory data analysis using multiple approaches
📁 Project Structure
Adult-Dataset-Analysis/
│
├── adult.csv
├── Adult_Dataset_Analysis.ipynb
├── sweetviz_report.html
└── README.md
🔗 Google Colab

The complete project and analysis can be viewed in Google Colab:

https://colab.research.google.com/drive/1mqVOHIiVGpvHOhx5_6j2-O0cWCB3N-rP?usp=sharing

👩‍💻 Author

Shandeepa 

B.Tech – Computer Science and Engineering

⭐ This project demonstrates practical experience in Python, Data Analysis, Data Cleaning, Exploratory Data Analysis, Data Visualization, and Automated EDA tools.

