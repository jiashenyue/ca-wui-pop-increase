# Drivers of population increase inside California's Wildland-Urban Interface (WUI)
- Shenyue Jia | [jiashenyue.info](https://jiashenyue.info)

## Overview of question
We will investigate what are the drivers/determining factors of **significant** population increase inside California's Wildland-Urban Interface (WUI), a high-risk area of wildfires in the transitioning zone from urban to wilderness.

## Target variable
- **Significant Mann-Kendall's tau (p < 0.05)**
  - Kendall’s Tau is a correlation suitable for quantitative and ordinal variables. 
  - It indicates how strongly 2 variables are monotonously related:
    - **to which extent are high values on variable x are associated with either high or low values on variable y?**
  - In this research question, variable x is years, variable y is population
    - A positive and high Kendall's tau population increase is strongly associated with the time
- **Steps to prepare the target variable**
  - [ ] Filter data to p < 0.05 for Mann-Kendall's tau
  - [ ] Filter data to Mann-Kendall's tau > 0

## Features
### Esri's House Affordability Index (HAI)
- **Meaning**
-  HAI measures the financial ability of a typical household to purchase an existing home in an area based on the share of income to mortgage
- **Steps to prepare the target variable**
  - [x] Already included in the original dataset

### Household Income
- **Steps to prepare the target variable**
  - [ ] Need to be retrieved from the Esri data
  - [ ] Calculate Max
  - [ ] Calculate Min
  - [ ] Calculate Median
  - [ ] Calculate Mean

### Rent-Own Ratio
- **Meaning**
  - Another metric to measure house affordability
    - High rent-own ratio means lower house affordability
- **Steps to prepare the target variable**
  - [ ] Need to be retrieved from the Esri data

### Wildfire Hazard Potential (WHP)
- **Meaning**
  - A measurement of the multi-year average of wildfire of a given census tract
    - High WHP means high wildfire risk
- **Steps to prepare the target variable**
  - [x] Already included in the original dataset
  - [ ] Calculate Max
  - [ ] Calculate Min
  - [ ] Calculate Median
  - [ ] Calculate Mean

### Wildfire Risk to Homes
- **Meaning**
  - A measure that integrates wildfire likelihood and intensity with generalized consequences to a home
- **Steps to prepare the target variable**
  - [ ] Need to be retrieved from data ([wildfirerisk.org](https://wildfirerisk.org/))
  - [ ] Calculate Max
  - [ ] Calculate Min
  - [ ] Calculate Median
  - [ ] Calculate Mean

### Percentage of area inside WUI
- **Meaning**
  - A measurement of wildfire risk
  - Higher percetentage inside WUI means a greater wildfire risk
- **Steps to prepare the target variable**
  - [ ] Need to be retrieved from the WUI data
