# LaQuinta Simple Linear Regression

Regression analysis to identify key predictors of hotel profitability and recommend expansion locations.

## Overview

This project analyzes factors influencing operating margins for LaQuinta hotel locations. Using exploratory analysis and linear regression, the goal is to determine which variables best predict profitability and whether a proposed new location meets the company's margin threshold.

## Dataset

- **Source:** LaQuinta hotel location data (SMB-A course dataset)
- **Observations:** Multiple hotel locations with operational and geographic data
- **Key variables:** Operating Margin (response), OfficeSpace, Number of competing rooms, Nearest competitor distance, College Enrollment, Median Income, Distance to downtown

## Methods

- Correlation analysis and scatterplot matrix (GGally)
- Simple Linear Regression (Margin ~ OfficeSpace)
- Multiple Linear Regression with variable selection
- 95% prediction interval for a proposed new location
- Diagnostic plots and residual analysis

## Key Findings

- **OfficeSpace** is the strongest single predictor of operating margin (positive relationship)
- **Number** of competing hotel rooms within 3 miles negatively impacts margin
- **Income** has a positive effect — higher median household income supports profitability
- Final model uses OfficeSpace, Number, Income, and Nearest as predictors

## Tools & Libraries

![R](https://img.shields.io/badge/R-276DC3?style=flat-square&logo=R&logoColor=white)
![tidyverse](https://img.shields.io/badge/tidyverse-1A162D?style=flat-square&logo=R&logoColor=white)
![GGally](https://img.shields.io/badge/GGally-276DC3?style=flat-square&logo=R&logoColor=white)

## How to Run

1. Clone the repository: `git clone https://github.com/BronsonBagwell/Simple_Linear_Regression.git`
2. Open `Simple_Linear_Regression.Rmd` in RStudio
3. Install required packages: `install.packages(c("tidyverse", "GGally"))`
4. Knit the document to reproduce the analysis
