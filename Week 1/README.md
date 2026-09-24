Superstore Sales Data Analysis (EDA)
📌 Project Overview
This project performs Exploratory Data Analysis (EDA) on the Sample Superstore dataset using Python. The main objective is to understand sales performance, identify business insights, and visualize the data through charts.

📂 Project Files
├── Task_1_BDA.ipynb              # Jupyter Notebook
├── task_1_bda.py                 # Python Script
├── samplesuperstore.csv          # Dataset
└── README.md                     # Project Documentation
📁 Dataset
Dataset Name: Sample Superstore

The dataset contains sales transactions from a retail superstore.

Main Columns
Order ID
Order Date
Ship Date
Customer Name
Segment
Country
City
State
Region
Category
Sub-Category
Product Name
Sales
Quantity
Discount
Profit
🛠 Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Jupyter Notebook
📚 Project Workflow
1. Import Required Libraries
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
Libraries are imported for data manipulation, analysis, and visualization.

2. Load Dataset
df = pd.read_csv("samplesuperstore.csv")
Reads the CSV file into a Pandas DataFrame.

3. Explore Dataset
df.head()
df.info()
df.describe()
These functions help understand the dataset structure, data types, and statistical summary.

4. Convert Date Columns
df['Order Date'] = pd.to_datetime(df['Order Date'])
df['Ship Date'] = pd.to_datetime(df['Ship Date'])
Converts date columns into datetime format for analysis.

5. Calculate Delivery Days
df['Delivery Days'] = (df['Ship Date'] - df['Order Date']).dt.days
Creates a new column showing the number of days taken for delivery.

6. Check Categories
df['Category'].unique()
Displays all product categories available in the dataset.

7. Check Missing Values
df.isnull().sum()
Checks whether the dataset contains any missing values.

8. Category-wise Sales Analysis
category_sales = df.groupby('Category')['Sales'].sum()
Calculates total sales for each product category.

9. Sales Bar Chart
category_sales.plot(kind='bar')
Visualizes total sales across different categories.

10. Sales Distribution
sns.histplot(df['Sales'], bins=30)
Displays the distribution of sales values using a histogram.

📈 Output
The project generates:

Dataset Overview
Statistical Summary
Delivery Days Calculation
Missing Value Report
Category-wise Sales Analysis
Sales Bar Chart
Sales Distribution Histogram
📌 Key Insights
Dataset is cleaned and explored.
Date columns are converted into datetime format.
Delivery time is calculated for each order.
Total sales are analyzed category-wise.
Sales distribution is visualized for better understanding.
▶️ How to Run
Clone this repository.
git clone <repository-link>
Install the required libraries.
pip install pandas numpy matplotlib seaborn
Run the notebook or Python file.
jupyter notebook Task_1_BDA.ipynb
or

python task_1_bda.py
📷 Sample Visualizations
Sales by Category (Bar Chart)
Sales Distribution (Histogram)
