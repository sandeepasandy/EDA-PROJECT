# 📊 Adult Dataset — Exploratory Data Analysis

> 🔍 A complete Exploratory Data Analysis project using Python, Data Visualization, and Automated EDA tools on the Adult Income Dataset.

---

## 🌟 Project Overview

This project focuses on performing **Data Cleaning, Data Preprocessing, Exploratory Data Analysis (EDA), and Data Visualization** using the `adult.csv` dataset.

The project combines traditional Python-based analysis with powerful **automated EDA tools** to explore the dataset, identify patterns, understand relationships between variables, detect missing values, analyze duplicates and outliers, and generate meaningful visualizations.

🚀 The project was developed using **Python and Google Colab**.

---

## 🎯 Objectives

The main objectives of this project are:

- 🧹 Perform data cleaning and preprocessing
- 🔍 Explore and understand the dataset
- ❓ Identify and handle missing values
- ♻️ Check duplicate records
- 📊 Analyze numerical and categorical variables
- 📈 Create meaningful visualizations
- 🔗 Analyze relationships and correlations
- ⚠️ Identify potential outliers
- 🤖 Explore automated EDA tools
- 📋 Generate automated dataset reports

---

## 📂 Dataset

### 📌 Adult Income Dataset

The `adult.csv` dataset contains demographic, educational, employment, and income-related information.

### 📊 Dataset Statistics

| Property | Details |
|---|---:|
| 📌 Records | 32,561 |
| 📌 Variables | 15 |
| 🔢 Numerical Variables | 6 |
| 🔤 Categorical Variables | 9 |
| 🎯 Target Variable | Income |

---

## 🧾 Dataset Features

Some of the important attributes include:

- 👤 Age
- 💼 Workclass
- 🎓 Education
- 🔢 Education Number
- 💍 Marital Status
- 🧑‍💼 Occupation
- 👨‍👩‍👧 Relationship
- 🌎 Race
- 🚻 Sex
- 💰 Capital Gain
- 💸 Capital Loss
- ⏰ Hours per Week
- 🌍 Native Country
- 💵 Income

---

# 🛠️ Technologies & Tools

### 🐍 Programming Language

- Python

### 📊 Data Analysis

- Pandas
- NumPy

### 📈 Data Visualization

- Matplotlib
- Seaborn
- Plotly

### 🤖 Automated EDA Tools

- D-Tale
- YData Profiling
- AutoViz
- Sweetviz

### ☁️ Development Environment

- Google Colab
- GitHub

---

# 🔄 Project Workflow

```text
📂 Dataset
     ↓
📥 Data Loading
     ↓
🔍 Data Exploration
     ↓
🧹 Data Cleaning
     ↓
❓ Missing Value Handling
     ↓
♻️ Duplicate Detection
     ↓
📊 Exploratory Data Analysis
     ↓
📈 Data Visualization
     ↓
🤖 Automated EDA
     ↓
📋 Reports & Insights
🔍 1. Data Loading

The dataset was loaded using Pandas.

import pandas as pd

data = pd.read_csv("adult.csv")
🔎 2. Data Exploration

The dataset was explored using different Pandas functions.

Operations performed:
head()
tail()
shape
columns
info()
describe()
dtypes
unique()
value_counts()

These operations helped understand the structure and characteristics of the dataset.

🧹 3. Data Cleaning

Several data-cleaning operations were performed.

🔹 Cleaning Operations
🔎 Identifying missing values
❓ Detecting ? values
♻️ Checking duplicate records
🔤 Checking data types
🧹 Handling missing data
📊 Checking categorical values
⚠️ Identifying possible outliers
❓ 4. Missing Value Handling

Different techniques were explored for handling missing values.

📌 Mean Imputation

Mean values can be used for suitable numerical columns.

data["column"].fillna(
    data["column"].mean(),
    inplace=True
)
📌 Mode Imputation

Mode can be used for suitable categorical columns.

data["column"].fillna(
    data["column"].mode()[0],
    inplace=True
)
📊 5. Exploratory Data Analysis

EDA was performed to understand the relationships and distributions within the dataset.

🔍 Areas explored:
👤 Age distribution
🎓 Education
💼 Workclass
🧑‍💼 Occupation
💰 Income
💍 Marital Status
👨‍👩‍👧 Relationship
⏰ Hours per Week
💵 Capital Gain
💸 Capital Loss
🌎 Native Country
📈 6. Data Visualization

Different Python visualization libraries were used.

📊 Matplotlib

Visualizations include:

📈 Line Charts
📊 Bar Charts
📉 Histograms
🔵 Scatter Plots
🎨 Seaborn

Visualizations include:

📊 Count Plots
📊 Bar Plots
📦 Box Plots
🔥 Heatmaps
📉 Distribution Plots
⚡ Plotly

Plotly was used to create interactive visualizations for better exploration of the dataset.

🤖 7. Automated EDA Tools

This project was extended using multiple automated EDA tools.

🖥️ D-Tale

D-Tale was used for interactive exploration of the Pandas DataFrame.

Features explored:
🔍 Data inspection
🔎 Filtering
↕️ Sorting
📊 Statistical analysis
📈 Visualization
🧾 DataFrame exploration
📋 YData Profiling

YData Profiling was used to generate an automated Adult Dataset Report.

The report provides:
📊 Dataset overview
🔢 Variable statistics
🔤 Variable types
❓ Missing-value analysis
♻️ Duplicate-row analysis
🔗 Correlations
📋 Sample data
⚠️ Data-quality alerts
Example:
from ydata_profiling import ProfileReport

profile = ProfileReport(
    data,
    title="Adult Dataset Report"
)

profile.to_notebook_iframe()
📊 AutoViz

AutoViz was used to automatically generate visualizations from the dataset.

The Income variable was used as the dependent variable.

AutoViz helped explore:
📊 Variable distributions
🔗 Relationships
📈 Scatter plots
⚠️ Outliers
🎯 Income-related patterns

The AutoViz analysis generated multiple visualizations automatically.

🍭 Sweetviz

Sweetviz was used to create an automated EDA report.

import sweetviz as sv

report = sv.analyze(data)

report.show_html(
    "sweetviz_report.html"
)
Sweetviz provides:
📊 Dataset overview
🔍 Variable analysis
📈 Distributions
🔗 Associations
📋 Automated visual reports
📸 Visualizations

The project contains visualizations created using:

📊 Matplotlib
        ↓
🎨 Seaborn
        ↓
⚡ Plotly
        ↓
🤖 AutoViz
        ↓
🍭 Sweetviz
        ↓
📋 YData Profiling
📊 Sample Visualizations

Add your generated chart screenshots here:

![Bar Chart](images/bar_chart.png)

![Line Chart](images/line_chart.png)

![Count Plot](images/count_plot.png)

![Heatmap](images/heatmap.png)
📋 Automated Reports

The project generates automated reports using:

Tool	Purpose
🖥️ D-Tale	Interactive DataFrame exploration
📋 YData Profiling	Detailed dataset profiling
📊 AutoViz	Automatic visualization
🍭 Sweetviz	Automated EDA report
💡 Key Learning Outcomes

Through this project, I learned how to:

🐍 Work with Python for data analysis
🐼 Use Pandas for dataset manipulation
🔢 Use NumPy for numerical operations
🧹 Clean and preprocess real-world datasets
❓ Handle missing values
♻️ Identify duplicate records
📊 Analyze categorical and numerical data
📈 Create different types of charts
🎨 Use Matplotlib and Seaborn
⚡ Create interactive visualizations using Plotly
🖥️ Explore datasets using D-Tale
📋 Generate profiling reports using YData Profiling
🤖 Automate visualization using AutoViz
🍭 Generate automated EDA reports using Sweetviz
🔗 Analyze correlations and relationships
⚠️ Understand outliers and data-quality issues
📁 Project Structure
Adult-Dataset-Analysis/
│
├── 📄 adult.csv
│
├── 📓 Adult_Dataset_Analysis.ipynb
│
├── 📊 sweetviz_report.html
│
├── 📁 images/
│   ├── 📊 bar_chart.png
│   ├── 📈 line_chart.png
│   ├── 📉 histogram.png
│   ├── 🔵 scatter_plot.png
│   └── 🔥 heatmap.png
│
└── 📖 README.md
🔗 Google Colab

🚀 Complete Project Notebook:

Open Project in Google Colab

📌 Project Highlights

✨ Real-world dataset analysis
🧹 Data cleaning & preprocessing
❓ Missing-value handling
♻️ Duplicate detection
📊 Exploratory Data Analysis
📈 Multiple visualization techniques
🤖 Automated EDA
📋 Automated profiling reports
🔍 Outlier & correlation analysis
🚀 Hands-on Python Data Analytics practice

👩‍💻 Author
Shandeepa 

🎓 B.Tech – Computer Science & Engineering

💻 Aspiring Data Analyst | Python | SQL | Data Analytics

⭐ If you found this project useful, feel free to explore the repository and give it a star!

🚀 Learning • Analyzing • Visualizing • Improving

