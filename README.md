### An Exploratory Analysis of Supply Chain Performance, Delivery Reliability and Order Economics

## Overview

This project explores supply chain operations using the DataCo Smart Supply Chain dataset. The analysis focuses on understanding delivery reliability, shipping efficiency, product sales performance, and profitability.

Rather than looking at sales figures alone, this project investigates operational patterns and business questions that can help identify potential inefficiencies in supply chain management.

## Objectives

- Analyze delivery performance across different shipping modes.
- Compare actual shipping durations with scheduled delivery expectations.
- Identify top-performing product categories by sales and profitability.
- Examine monthly sales trends and changes in order composition.
- Investigate the relationship between discount rates and profitability.
- Identify data quality issues, missing values, and unusual patterns.

## Dataset

**Dataset:** DataCo Smart Supply Chain for Big Data Analysis

**Source:** [Kaggle – DataCo Smart Supply Chain Dataset](https://www.kaggle.com/datasets/shashwatwork/dataco-smart-supply-chain-for-big-data-analysis)

The dataset contains 180,519 records and 53 columns, covering order transactions, customers, products, shipping information, and financial metrics.

The primary file used in this analysis is `DataCoSupplyChainDataset.csv`.

The raw dataset is not included in this repository. Download it from Kaggle before running the notebook.

## Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Google Colab / Jupyter Notebook

## Analysis Workflow

1. **Data Understanding:** Examined dataset dimensions, column types, memory usage, and sample records.
2. **Data Quality Assessment:** Investigated missing values, duplicate records, constant columns, and redundant features.
3. **Data Preparation:** Converted date columns into appropriate datetime formats and created an order-level dataset for delivery analysis.
4. **Exploratory Data Analysis:** Investigated delivery performance, shipping durations, category sales, monthly trends, discounts, and profitability.
5. **Business Insights:** Summarized significant operational and financial patterns observed in the data.

## Visualizations and Analysis

The notebook includes eight visualizations:

1. Distribution of orders by delivery status.
2. Late delivery rate across shipping modes.
3. Actual versus scheduled shipping days by shipping mode.
4. Top 10 product categories by total sales.
5. Monthly sales trend from 2015 to 2018.
6. Average profitability across discount ranges.
7. Top 10 product categories by average recorded profit.
8. Distribution of profitable, loss-making, and zero-profit order items.

## Key Findings

- **Delivery reliability:** Approximately 54.82% of unique orders are classified as late deliveries, while only 17.83% are classified as shipping on time.
- **Shipping performance:** First Class has a 95.3% late delivery rate, compared with 38.1% for Standard Class.
- **Order composition:** Average items per order decline from approximately 3 in September 2017 to 1 in November 2017. This coincides with a substantial decline in monthly sales.
- **Discount and profitability:** Average recorded profit decreases from 23.94 in the 0–5% discount range to 18.41 in the 20–25% range.
- **Category profitability:** Fishing generates the highest total sales, while Computers has the highest average recorded profit per order item.
- **Loss-making items:** Approximately 18.72% of order items have negative recorded profit.

## Important Considerations

- Delivery analysis uses unique orders to avoid counting multi-item orders multiple times.
- Product sales and profitability analysis uses individual order-item records.
- The late-2017 sales decline requires further validation because order composition changes substantially during this period.
- The analysis identifies associations, not causal relationships.
- Some columns contain substantial missing values, redundant information, or constant values.
- Customer-related personal information is excluded from the analysis.

## How to Run the Project

1. Clone or download this repository.
2. Download the dataset from the Kaggle link provided above.
3. Extract the dataset and place `DataCoSupplyChainDataset.csv` inside a folder named `data`.
4. Open `Supply_Chain_Performance_EDA.ipynb` in Google Colab or Jupyter Notebook.
5. Run the notebook cells sequentially.

Expected dataset path:

`data/DataCoSupplyChainDataset.csv`

The notebook uses Latin-1 encoding to read the CSV file.

## Project Structure

```text
Supply-Chain-Performance-Analysis/
│
├── Supply_Chain_Performance_EDA.ipynb
├── README.md
└── .gitignore
```

## Conclusion

This exploratory analysis highlights how supply chain performance involves more than revenue generation. Delivery reliability, shipping expectations, order composition, discounting, and product profitability all contribute to understanding operational and financial performance.

The findings provide a foundation for further investigation into delivery optimization and profitability improvement.

---

**Project Type:** Exploratory Data Analysis (EDA)  
**Domain:** Supply Chain Analytics  
**Author:** Chinmay Mohite
