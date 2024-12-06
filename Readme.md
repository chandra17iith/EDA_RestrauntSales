# Restaurant Sales Data - Exploratory Data Analysis (EDA)

## Project Overview

This project involves performing an Exploratory Data Analysis (EDA) on a dataset of sales transactions from a fast-food restaurant. The goal is to identify key trends, popular items, revenue patterns, and customer behavior based on transaction types and gender. The analysis includes data cleaning, visualization, and time-based revenue insights.

---

## Dataset Overview

The dataset contains sales transactions with the following key features:

- **transaction_amount**: Total value of each transaction.
- **item_type**: Type of the item sold (e.g., Fastfood or Beverages).
- **item_name**: Name of the specific item sold.
- **transaction_type**: Mode of transaction (Online or Offline).
- **received_by**: Gender of the customer (Male/Female).
- **date**: Date of the transaction.
- **time_of_sale**: Time of the transaction (Morning, Afternoon, Evening, Night).

---

## Key Steps in Analysis

### 1. Data Loading and Cleaning
- **Missing Values**: Filled missing values in the `transaction_type` column with "Online".
- **Gender Classification**: Replaced titles (`Mr.`/`Mrs.`) in the `received_by` column with `Male`/`Female`.
- **Date Formatting**: Reformatted the `date` column into a consistent format and created a `Month-Year` column for time-based analysis.

### 2. Univariate Analysis
- **Transaction Amount Distribution**: A histogram was used to analyze the distribution of transaction amounts, which revealed that most transactions were below 400 rupees.
- **Item Prices**: Average prices of items in the Fastfood and Beverages categories were calculated.

### 3. Bivariate Analysis
- **Revenue and Quantity by Item Type**: Grouped the data by `item_type` and `item_name` to analyze which items contributed the most in terms of both revenue and quantity.
- **Visualizations**: Bar plots revealed that fast food items like sandwiches and frankies contribute the most revenue, while items like panipuri and vadapav have high sales quantities but generate less revenue due to lower prices.

### 4. Time-Based Analysis
- **Monthly Revenue Trends**: A line chart showed the revenue trends across different months. This highlighted peak months and allowed for analysis of revenue patterns over time.
- **Item-Level Time Trends**: Time-based analysis for specific fast food and beverage items (e.g., sandwiches, frankies, cold coffee) helped understand their revenue trends over different months.

### 5. Sales by Time of Day
- **Time of Sale Analysis**: Sales performance was analyzed based on different times of the day (morning, afternoon, evening, night), revealing interesting patterns of when items were most popular.

### 6. Transaction Type and Gender-Based Analysis
- **Transaction Type**: Compared revenue from online vs offline sales using pie charts.
- **Gender Sales Distribution**: Analyzed the sales distribution by gender using pie charts to show which gender contributed more to the restaurant's revenue.

---

## Visualizations

- **Histograms**: Used to show the distribution of `transaction_amount` values.
- **Bar Plots**: Used to compare revenue and quantity sold across different item types.
- **Line Charts**: Analyzed monthly revenue trends for the restaurant and specific items.
- **Pie Charts**: Used to show the distribution of revenue by transaction type and gender.
- **Correlation Matrix (Optional)**: A heatmap could be added to show correlations between numerical features like `quantity` and `transaction_amount`.

---

## How to Run the Project

### Prerequisites

Ensure that you have the following Python libraries installed in your environment:

```bash
pip install pandas numpy matplotlib seaborn
```
---
## Running the Code

There are two ways to run the analysis:

1. Jupyter Notebook:
Open the EDA_restaurantSales.ipynb notebook.
Run the cells to perform each step of the analysis interactively.

2. Python Script:
To run the analysis as a script, execute the eda_restaurantSales.py file using Python:

---
## Imporvement and Future Work
1. Outlier Detection: Detect and handle outliers in the `transaction_amount` column to improve the accuracy of the analysis.
2. Correlation Matrix: Explore correlations between numerical columns such as `quantity` and `transaction_amount`.
3. Predictive Modeling: Use machine learning models to predict future sales based on historical data.
4. Customer Behavior Analysis: Investigate customer trends, including repeat customer behavior or loyalty analysis.

---
## Conclusion

This exploratory data analysis provided valuable insights into the sales trends at a fast-food restaurant. The analysis revealed top-selling items, time-based revenue patterns, and customer preferences based on transaction and gender types. Further improvements can focus on predictive analytics and deeper customer behavior studies.
