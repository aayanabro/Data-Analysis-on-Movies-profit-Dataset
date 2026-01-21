# 🎬 Movie Industry Profitability Analysis

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Library-Pandas-orange)](https://pandas.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Library-Matplotlib-green)](https://matplotlib.org/)

## 📌 Project Overview
This project performs an Exploratory Data Analysis (EDA) on a movie profitability dataset to identify patterns between production costs and global revenue. The goal is to determine which factors—such as **Genre**, **MPAA Rating**, or **Distributor**—most significantly impact a film's financial success.

---

## 🛠️ Tech Stack & Libraries
The analysis is built using the following Python ecosystem:
* **Data Manipulation**: `Pandas`
* **Data Visualization**: `Matplotlib`, `Seaborn`
* **Environment**: Google Colab / Jupyter Notebook

---

## 📊 Data Processing Workflow

### 1. Data Cleaning
* **Index Removal**: Dropped the redundant `Unnamed: 0` column to clean the feature set.
* **Handling Nulls**: Utilized `dropna()` to remove incomplete records, ensuring high-quality statistical output.
* **Sorting**: Ordered data by `production_budget` to observe trends from independent films to massive blockbusters.

### 2. Exploratory Analysis
The code performs deep-dive aggregations to uncover:
* **Genre Insights**: Calculates mean production budgets and maximum domestic gross per genre.
* **Rating Impact**: Analyzes how MPAA ratings (G, PG, PG-13, R) correlate with domestic median and mean gross.
* **Distributor Performance**: Sums and averages worldwide gross to identify the most successful studios.

### 3. Visualizations Generated
The script produces several key plots to communicate findings:
* **Histograms**: Distribution of Worldwide Gross.
* **Time-Series**: Line plot showing the mean of Worldwide Gross over the years (using date slicing).
* **Composition**: Pie chart of Total Domestic Gross by MPAA Rating.
* **Correlations**: Scatter plot of Production Budget vs. Domestic Gross to identify ROI.
* **Rankings**: Horizontal bar charts for Distributor performance.

---

## 🚀 Getting Started

### Prerequisites
Ensure you have the dataset `movie_profit.csv` in your local directory or Colab environment.

### Installation
```bash
pip install pandas matplotlib seaborn
