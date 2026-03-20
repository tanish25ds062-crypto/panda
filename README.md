📊 Pandas Basics Notebook
📌 Overview

This notebook introduces Pandas, a powerful Python library used for working with structured data. It covers essential concepts like data creation, manipulation, filtering, and analysis.

Pandas is widely used in:

Data Analysis

Data Cleaning

Machine Learning preprocessing

Working with CSV/Excel data

⚙️ Installation
pip install pandas
📥 Import Library
import pandas as pd
🧱 What is Pandas?

Pandas is a Python library used for handling structured data in the form of tables (like Excel or SQL tables).

📊 What is a DataFrame?

A DataFrame is a 2D table with rows and columns.

🚀 Topics Covered
1️⃣ Creating DataFrames

From Lists

From Dictionary

df = pd.DataFrame([11,22,33], columns=['Col_Name'])
data = {
    'Name': ['Madhav', 'Vishakha'],
    'Age': [16,17]
}
df = pd.DataFrame(data)
2️⃣ Understanding DataFrame

head(), tail()

shape

columns

info()

describe()

3️⃣ File Handling

Save to CSV

Load from CSV

df.to_csv('file.csv', index=False)
df = pd.read_csv('file.csv')
4️⃣ Selecting Data

Single & multiple columns

Rows using loc and iloc

df[['Name']]
df.loc[0:2]
df.iloc[0:2]
5️⃣ Filtering Data

Conditions

Multiple filters

where() function

df[df['Age'] >= 18]
6️⃣ Data Operations

Add column

Update values

Delete rows/columns

Sorting

df['Bonus'] = df['Salary'] * 0.2
df.drop('Bonus', axis=1)
df.sort_values('Salary')
7️⃣ Working with Dates

Convert to datetime

Extract year, month, day

df['DOJ'] = pd.to_datetime(df['DOJ'])
df['DOJ'].dt.year
🎯 Key Learnings

How to create and manipulate DataFrames

Filtering and selecting data efficiently

Handling CSV files

Working with date-time data

Performing basic data analysis

📁 File Included

Pandas.ipynb → Main notebook with examples

💡 Who is this for?

Beginners in Data Science

Python learners

Students starting with Pandas

🙌 Author Note

This notebook is beginner-friendly and designed to build strong fundamentals in Pandas.
