# Exploratory Data Analysis with Python – Tips Dataset

## Overview
This project demonstrates **Exploratory Data Analysis (EDA)** using Python on the **Tips Dataset**. The objective of this analysis is to understand the structure of the dataset, explore patterns in the data, detect potential outliers, and analyze relationships between variables using visualizations.

EDA is an important step in data analysis as it helps analysts gain insights into data distributions, identify anomalies, and uncover relationships between variables before performing further statistical analysis or modeling.

The analysis in this notebook includes:
- Distribution analysis using histograms
- Outlier detection using box plots and Interquartile Range (IQR)
- Multi-variable comparison using interactive visualizations

---

## Dataset Information

**Dataset:** Tips Dataset  
**Source:** Seaborn Built-in Dataset (GitHub)  
**Direct Link:**  
https://raw.githubusercontent.com/mwaskom/seaborn-data/master/tips.csv

The dataset contains **244 restaurant transactions** recorded by a waiter over several months.

Each row represents one dining transaction with information about the total bill, tip amount, customer characteristics, and dining context.

### Dataset Columns

| Column | Description |
|------|-------------|
| total_bill | Total bill amount in USD |
| tip | Tip amount given in USD |
| sex | Gender of the bill payer |
| smoker | Whether the table had a smoker (Yes/No) |
| day | Day of the week (Thur, Fri, Sat, Sun) |
| time | Meal time (Lunch or Dinner) |
| size | Number of people at the table |

---

## Project Objectives

The main objectives of this exploratory analysis are:

1. **Understand Data Distribution**
   - Analyze how restaurant bill amounts are distributed using histograms.

2. **Identify Outliers**
   - Use box plots and the Interquartile Range (IQR) method to detect unusual values in bill amounts across different days.

3. **Explore Relationships Between Variables**
   - Examine how tip amounts relate to total bill values.
   - Compare tipping patterns between lunch and dinner transactions using an interactive scatter plot.

---

## Tasks Performed

### Task 1: Distribution Analysis
Two histograms were created for the **total_bill** variable using different bin sizes (5 and 20 bins).  
This helps visualize how bill values are distributed and understand the impact of bin selection on data interpretation.

### Task 2: Outlier Detection
Box plots were used to compare total bill distributions across days of the week (Thursday, Friday, Saturday, and Sunday).  
The **Interquartile Range (IQR)** method was applied to manually calculate outlier boundaries and verify unusual observations.

### Task 3: Multi-Variable Comparison
An interactive scatter plot was created using **Plotly** to analyze the relationship between **total_bill and tip**.  
Points are colored based on meal time (Lunch or Dinner), and hover labels display additional information such as the day and table size.

---

## Technologies Used

- Python
- Pandas
- Matplotlib
- Seaborn
- Plotly
- Jupyter Notebook

---

## Key Insights

- The **total bill distribution is right-skewed**, indicating that most restaurant bills fall within a lower to moderate price range, while a few bills are significantly higher.
- **Saturday generally shows the highest median total bill**, suggesting higher spending during weekend dining.
- The analysis reveals a **positive relationship between total bill and tip amount**, meaning tips generally increase as the bill amount increases.
- Dinner transactions tend to involve **higher bills and tips compared to lunch transactions**.

---

## Repository Structure
eda-assignment/
│
├── EDA_Assignment_YourName.ipynb
└── README.md


---

## How to Run the Notebook

1. Clone the repository:
https://github.com/J-harshavardhan/eda-assignment.git


2. Navigate to the project directory:
cd eda-assignment


3. Open the notebook using Jupyter:
jupyter notebook


4. Run all cells to reproduce the analysis and visualizations.

---

## Author

**Jagannati Harshavardhan**

This project was completed as part of an assignment on **Exploratory Data Analysis using Python**.
