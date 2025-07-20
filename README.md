# 📊 Exploratory Data Analysis (EDA) – Book Price Dataset
## 🧾 Overview
This project performs Exploratory Data Analysis (EDA) on book data scraped from https://books.toscrape.com. The dataset contains book titles, prices, and availability. EDA helps understand the data structure, identify trends, detect anomalies, and prepare the data for future use in machine learning or reporting.

## 📁 Dataset Details
Filename: books_dataset.csv Columns:

Title: Book name

Price: Price in GBP (as float)

Availability: Stock status (string)

InStock: Boolean column derived from availability

## ✅ Project Goals
Clean and prepare the raw dataset

Understand the distribution of prices

Identify and handle anomalies (e.g., outliers, duplicates)

Explore stock availability

Generate visual insights

## 📦 Libraries Used
| Library       | Purpose                         |
| ------------- | ------------------------------- |
| `pandas`      | Data loading, transformation    |
| `matplotlib`  | Plotting graphs                 |
| `seaborn`     | Statistical data visualization  |
| `scipy.stats` | Outlier detection using z-score |

## 🚀 Getting Started
1. Install Required Libraries
```bash
pip install pandas matplotlib seaborn scipy
```
2. Run the EDA Notebook or Script

You can use:

Jupyter Notebook

Python Script

## 🔍 Key Steps Performed
1. Load and Explore
Previewed top rows using head()

Checked column types and structure with info()

Summarized data with describe()

2. Clean the Data
Removed duplicates

Converted price from string to float

Normalized availability status

Created InStock boolean column

Capped outlier prices above the 95th percentile

3. Detect Anomalies
Used boxplots and z-scores to detect extreme prices

Checked for nulls and duplicates

Visualized stock availability distributions

4. Visualizations
Histogram of price distribution

Countplot of books in vs out of stock

Boxplot of price outliers

Price comparison by availability

## 📤 Output
Cleaned dataset: books_dataset_cleaned.csv

Plots and insights in eda_books.ipynb

## 📌 File Structure
```bash
book-eda/
├── books_dataset.csv             # Original dataset
├── books_dataset_cleaned.csv     # Cleaned output
├── eda_books.ipynb               # Jupyter EDA notebook
├── eda_books.py                  # Python EDA script
└── README.md                     # This file
```
