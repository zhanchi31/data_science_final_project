# data_science_final_project

# NYC Air Quality and Public Health Analysis

## Project Overview

This project analyzes air quality and public health indicators in New York City from 2009 to 2023. The main focus is to understand how major air pollutants, including PM2.5, nitrogen dioxide (NO2), and ozone (O3), vary across geographic areas and how these indicators are related to public health outcomes.

The project includes data preprocessing, exploratory data analysis, visualization, spatial comparison, and time-series forecasting.

## Research Objectives

The main objectives of this project are:

1. To clean and prepare NYC air quality and health impact data for analysis.
2. To explore major environmental indicators such as PM2.5, NO2, and Ozone.
3. To compare pollution patterns across different geographic areas.
4. To examine possible relationships between air pollution and public health outcomes.
5. To forecast future air quality trends using time-series models.

## Data Source

The dataset used in this project is based on NYC air quality and health impact data at different geographic levels, including UHF42, borough, community district, and citywide levels.

Main data files used in this project:

- `Air_Quality_and_Health_Impacts_20260423.csv`: original raw dataset
- `Air_Quality_and_Health_Impacts_processed.csv`: cleaned and processed dataset
- `Time_Trend.csv`: time-series dataset used for forecasting

The dataset contains information such as:

- Indicator name
- Measure type
- Geographic area
- Time period
- Start date
- Data value
- Pollution and health-related measurements

## Project Structure

```text
├── README.md
├── Air_Quality_and_Health_Impacts_20260423.csv
├── Air_Quality_and_Health_Impacts_processed.csv
├── Time_Trend.csv
├── Data preprocessing.Rmd
├── Data Overall.Rmd
├── Data Time_Trend.Rmd
├── Plot1_Top_Indicators.png
├── Plot2_PM25_Income_Equity.png
├── Plot3_Correlation_Matrix.png
└── Plot4_PM25_Raincloud.png
```

## Required R Packages

The project uses the following R packages:

```r
install.packages(c(
  "tidyverse",
  "lubridate",
  "e1071",
  "scales",
  "ggcorrplot",
  "tsibble",
  "fable",
  "feasts",
  "ggdist",
  "viridis",
  "knitr"
))
```

After installing the packages, load them in R:

```r
library(tidyverse)
library(lubridate)
library(e1071)
library(scales)
library(ggcorrplot)
library(tsibble)
library(fable)
library(feasts)
library(ggdist)
library(viridis)
library(knitr)
```

## How to Run the Project

### Step 1: Download or clone the repository

Clone this repository or download all project files into one folder.

### Step 2: Open the project in RStudio

Open the project folder in RStudio and make sure all CSV files and R Markdown files are in the same working directory.

### Step 3: Run the preprocessing notebook

Run:

```text
Data preprocessing.Rmd
```

This notebook performs:

- Initial data exploration
- Missing value checking
- Outlier detection
- Date transformation
- Feature engineering
- Geographic cleaning
- Export of processed datasets

It creates the processed files:

```text
Air_Quality_and_Health_Impacts_processed.csv
Time_Trend.csv
```

### Step 4: Run the overall analysis notebook

Run:

```text
Data Overall.Rmd
```

This notebook generates:

- Summary statistics
- Top environmental indicator chart
- PM2.5 spatial comparison
- Correlation matrix
- Raincloud plot
- Summary tables

### Step 5: Run the time-trend forecasting notebook

Run:

```text
Data Time_Trend.Rmd
```

This notebook performs:

- Time-series data preparation
- ARIMA model fitting
- ETS model fitting
- Backtesting using 2020-2023 data
- Forecasting for 2024-2028

## Main Methods

This project uses the following methods:

- Exploratory Data Analysis
- Missing value analysis
- IQR-based outlier detection
- Log transformation for highly skewed variables
- Correlation analysis
- Spatial comparison
- Time-series forecasting
- ARIMA and ETS models

## Key Outputs

The main outputs include:

- Cleaned dataset
- Processed time-series dataset
- Descriptive statistics tables
- Pollution distribution visualizations
- Correlation matrix
- Forecasting comparison plot

## Authors

- Lei Wei
- Minghao Lu
- Junbo Zhang
- Weizhan Gao
- Jiaqi Li

University of Arizona  
DATA 498 Final Project
