# Retail Sales Data Analysis

## Overview

This project analyzes a retail sales dataset using Python, Pandas, Matplotlib, and Seaborn. It demonstrates data analysis skills through data cleaning, exploratory data analysis (EDA), visualizations, and deriving actionable insights. The project is built in Google Colab, with the dataset loaded from Google Drive 

## Dataset

- **Source**: Retail Sales Dataset on Kaggle
- **Description**: A synthetic dataset of retail transactions with \~1,000 rows, including customer demographics, product categories, and sales data.
- **Columns**:
  - `Transaction ID`: Unique transaction identifier (integer)
  - `Date`: Transaction date (string, e.g., 'YYYY-MM-DD')
  - `Customer ID`: Unique customer identifier (string)
  - `Gender`: Customer gender (categorical: 'Male', 'Female')
  - `Age`: Customer age (integer)
  - `Product Category`: Product category (e.g., 'Electronics', 'Clothing', 'Beauty')
  - `Quantity`: Number of items purchased (integer)
  - `Price per Unit`: Price per item (float)
  - `Total Amount`: Total sale amount (float, Quantity \* Price per Unit)

## Prerequisites

- **Python Libraries**: `pandas`, `matplotlib`, `seaborn`
- **Environment**: Google Colab or Jupyter Notebook
- **Google Drive**: Mount Google Drive in Colab to access the dataset

## Setup Instructions

1. **Install Dependencies**:

   ```bash
   pip install pandas matplotlib seaborn kaggle
   ```
2. **Dataset Setup**:
   - **Option 1: Manual Upload**:
     - Download `retail_sales_dataset.csv` from the Kaggle dataset link.
     - Upload it to your Google Drive (e.g., `/MyDrive/Github Projects/retail_sales_dataset.csv`).
   2. **Run the Notebook**:
   - Open `analysis.ipynb` in Google Colab.
   - Ensure Google Drive is mounted:

     ```python
     from google.colab import drive
     drive.mount('/content/drive')
     ```
   - Load the dataset from `/content/drive/MyDrive/Github Projects/retail_sales_dataset.csv`.
   - Run all cells to perform cleaning, visualizations, and insights.

## Project Structure

- `analysis.ipynb`: Jupyter Notebook with the full analysis (data loading, cleaning, visualizations, insights).
- `retail_sales_dataset.csv`: The dataset (included in repo or downloadable via Kaggle API).
- `README.md`: This file.
- `requirements.txt`: List of required Python libraries.
- `plots/` : Folder for saved visualization images.

## Analysis Steps

1. **Data Loading**: Load `retail_sales_dataset.csv` from Google Drive.
2. **Data Cleaning**:
   - Convert `Date` to datetime.
   - Check for missing values and duplicates.
   - Add a `Month-Year` column for time-based analysis.
3. **Visualizations**:
   - Bar plot: Total sales by product category.
   - Box plot: Sales distribution by gender.
   - Line plot: Total sales over time (monthly).
   - Histogram: Customer age distribution.
   - Heatmap: Correlation between numerical features.
4. **Insights**:
   - Top-selling product category.
   - Average spend by gender.
   - Most common customer age.
   - Total overall sales.
   - Peak sales month.

## Results

- Visualizations reveal sales trends, customer demographics, and correlations.
- Key insights include top-performing product categories and spending patterns by gender and age.


## Screenshots
<img src="plots/barplot.png" alt="Sales by Category(barplot)" width="500">
<img src="plots/boxplot.png" alt="Sales by Gender" width="500">
<img src="plots/histogram.png" alt="Age Distribution" width="500">
<img src="plots/lineplot.png" alt="Sales Over Time" width="500">
<img src="plots/heatmap.png" alt="Correlation Heatmap" width="500">



## License

MIT License