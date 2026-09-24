Task 1 - Business Data Analysis
📌 Project Overview
This project performs exploratory data analysis (EDA) on a Superstore dataset using Python.

The analysis focuses on understanding sales, profit, product categories, discounts, delivery time, and relationships between numerical variables through data analysis and visualization.

🛠️ Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Google Colab / Jupyter Notebook
📂 Project Files
task_1_bda_(2).py — Python source code
Task_1_BDA_(2).ipynb — Google Colab/Jupyter Notebook
samplesuperstore.csv — Dataset required to run the analysis
🔍 Analysis Performed
The project includes the following steps:

1. Data Loading and Inspection
The Superstore CSV dataset is loaded using Pandas. Initial data inspection is performed using:

head()
info()
describe()
Missing-value checking
Unique category identification
2. Data Preprocessing
The Order Date and Ship Date columns are converted into datetime format.

A new column called Delivery Days is calculated to determine the number of days between the order date and shipping date.

3. Sales Analysis
Sales are grouped by product category to examine total sales for each category.

A bar chart is created to visualize Sales by Category.

4. Sales Distribution
A histogram is used to visualize the distribution of sales values across the dataset.

5. Profit Analysis
Profit is analyzed across different product categories using bar charts.

Box plots are also used to examine:

Overall profit distribution
Profit variation across categories
6. Discount and Profit Analysis
A scatter plot is created to investigate the relationship between Discount and Profit.

This helps visualize how different discount levels are associated with profit values.

7. Correlation Analysis
Numerical columns are selected and a correlation matrix is calculated.

A heatmap is then created to visualize relationships between numerical variables.

📊 Visualizations
The project generates several visualizations, including:

Sales by Category
Sales Distribution
Profit by Category
Sales Distribution by Category
Profit Distribution
Profit Variation Across Categories
Impact of Discount on Profit
Correlation Heatmap
These visualizations are created using Matplotlib and Seaborn.

▶️ How to Run
Option 1: Google Colab
Upload the .ipynb file to Google Colab.
Upload samplesuperstore.csv to the Colab environment.
Run the notebook cells sequentially.
Option 2: Jupyter Notebook
Install the required libraries:

pip install pandas numpy matplotlib seaborn
Then open:

Task_1_BDA_(2).ipynb
and run the cells.

Option 3: Python
Make sure the dataset path in the Python file points to your local samplesuperstore.csv file.

Then run:

python task_1_bda_(2).py
📁 Recommended GitHub Structure
Task-1-BDA/
│
├── README.md
├── task_1_bda_(2).py
├── Task_1_BDA_(2).ipynb
└── samplesuperstore.csv
🎯 Objective
The main objective of this project is to apply basic Business Data Analytics techniques to a real-world-style sales dataset and understand business performance through data exploration and visualization.


