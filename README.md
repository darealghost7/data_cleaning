# data_cleaning

# Concert Tour Data Analysis

This project performs comprehensive data cleaning and exploratory analysis on a dataset of the highest-grossing concert tours of all time.

## Overview

This Jupyter notebook contains a complete data cleaning pipeline and exploratory analysis of concert tour data, including handling missing values, outlier detection, and grouping operations to extract insights about tour performances.

## Key Features

- **Data Loading**: Imports tour data from CSV file
- **Data Manipulation**: Sorting, filtering, and creating new calculated columns
- **Missing Value Handling**: Identification and treatment of null values using fillna() and dropna()
- **Duplicate Removal**: Deduplication based on artist names
- **Outlier Detection**: Both IQR (Interquartile Range) and Z-score methods
- **Statistical Analysis**: Summary statistics using describe() and groupby operations

## Dataset Information

The dataset contains information about top-grossing concert tours including:
- Tour rankings and peak positions
- Gross revenue (actual and inflation-adjusted)
- Artist names
- Tour titles
- Year(s) of tour
- Number of shows
- Average gross per show
- References

## Key Analyses Performed

1. **Sorting Operations**
   - Tours sorted by number of shows and artist name

2. **Filtering**
   - Tours with more than 130 shows identified
   - Tours with more than 100 shows flagged in new column

3. **Missing Data**
   - Null value counts calculated
   - Missing values filled with zeros
   - Selected column missing values filled with mean

4. **Duplicate Detection**
   - Duplicate entries removed based on Artist column

5. **Outlier Detection**
   - IQR method: Identified outlier bounds
   - Z-score method: Tours with Z-score > 3 flagged as outliers

6. **Group Operations**
   - Mean shows by new column flag
   - Mean shows by artist
   - Mean shows by artist and year(s)

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy

## Getting Started

1. Ensure you have the required libraries installed:
```bash
pip install pandas numpy matplotlib seaborn scipy
