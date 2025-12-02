# Earthquake Frequency and Magnitude vs Population Analysis

## Project Overview
This project analyzes the relationship between city population and earthquake frequency in the Philippines. We use earthquake data and population data to determine whether larger cities experience more earthquakes.

## Folder Structure
Datasets/
Cleaned Datasets/
Final_Data.csv # Final dataset with cleaned data for analysis
Merged_DS.csv # Merged dataset of earthquake and population data
year_stats.csv # Yearly earthquake stats (min, max magnitude, frequency)
Original Datasets/
phivolcs_earthquake_data.csv # Original earthquake data 
phl_population-2020_2025.csv # Original population data (CSV format)
phl_population-2020_2025.xlsx # Original population data (Excel format)
Python Codes/
Techtators_Cleaning.ipynb # Data cleaning and preprocessing script
Techtators_Corr_Normalization.ipynb # Correlation and normalization analysis

## Code Explanation
- **Techtators_Cleaning.ipynb**:
  1. Loads and cleans the population and earthquake datasets.
  2. Merges the datasets by city.
  3. Creates a new dataset with earthquake statistics by year and city.
  4. Saves the cleaned datasets (`Final_Data.csv`, `year_stats.csv`).

- **Techtators_Corr_Normalization.ipynb**:
  1. Loads the cleaned datasets.
  2. Calculates the correlation between population and earthquake frequency.
  3. Creates visualizations (scatter plots, heatmaps) of the data.
  4. Applies normalization to the data and recalculates correlation.

