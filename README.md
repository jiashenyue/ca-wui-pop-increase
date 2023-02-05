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
  - Filter data to p < 0.05 for Mann-Kendall's tau
  - Filter data to Mann-Kendall's tau > 0

## Features
### Esri's House Affordability Index (HAI)
- 
