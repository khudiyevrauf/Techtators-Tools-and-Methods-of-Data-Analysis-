# Earthquake Frequency and Magnitude vs Population Analysis

## Project Overview
This project investigates the relationship between city population and earthquake frequency in the Philippines. The analysis leverages data from PHIVOLCS (Philippine Institute of Volcanology and Seismology) for earthquakes and population data for cities in the Philippines and Datasets were taken from Kaggle. The aim is to explore whether larger cities experience more frequent or more intense earthquakes.

The project integrates 2 datasets, including population figures for cities in the Philippines and earthquake data over several years. It uses data cleaning, merging, correlation analysis, and data visualization techniques to uncover insights.

## Folder Structure

Python Codes/

Techtators_Cleaning.ipynb # Data cleaning and preprocessing script

Techtators_Corr_Normalization.ipynb # Correlation and normalization analysis

CSV and XLSX files which are hidden with gitignore

requirements.txt # List of dependencies for the project

README.md # Project documentation (this file)

.gitignore # with codes ignoring csv and xlsx

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

## Integration Strategy
### 1. Data Collection:

The project starts by collecting the raw:

Earthquake Data: This data contains information about earthquakes in the Philippines, including their location, magnitude, and date.

Population Data: The population data for Philippine cities is collected for the years 2020–2025.

### 2. Data Cleaning:

Techtators_Cleaning.ipynb is used to clean the data:

The column names are standardized (e.g., Municipality_City is changed to City).

The city names are cleaned by stripping extra spaces and converting them to lowercase.

The dataset is filtered to exclude specific years (2016–2019) based on the project needs.

### 3. Merging Datasets:

The cleaned population data is merged with the earthquake data based on the City column.

This results in a new merged dataset (Merged_DS.csv), which combines the earthquake and population information for analysis.

### 4. Data Aggregation:

From the merged dataset, yearly statistics (e.g., min/max earthquake magnitudes, earthquake frequency per year) are calculated and saved into year_stats.csv.

### 5. Correlation Analysis & Normalization:

Techtators_Corr_Normalization.ipynb performs a Pearson correlation analysis between the city population and earthquake frequency.

Normalization: Both population and earthquake frequency data are normalized using MinMaxScaler to bring the values into the same scale.

### 6. Visualization:

Visualizations such as scatter plots, heatmaps, and trendlines are generated to better understand the relationship between the variables.

### 7. Final Dataset:

The final dataset, Final_Data.csv, contains the cleaned and merged data, ready for any additional analysis or modeling.

This dataset is used for analysis and correlation studies.
