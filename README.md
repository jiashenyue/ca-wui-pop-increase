# Drivers of population increase inside California's Wildland-Urban Interface (WUI)
- Shenyue Jia | [jiashenyue.info](https://jiashenyue.info)

## Overview of question
We will investigate what are the drivers/determining factors of **significant** population increase inside California's Wildland-Urban Interface (WUI), a high-risk area of wildfires in the transitioning zone from urban to wilderness.

## Target variable
- `percent_pop_change` column
  - Annualized percentage of population change based on data from 2010 to 2019

## Features
### Esri's House Affordability Index (HAI)
- **Meaning**
-  HAI measures the financial ability of a typical household to purchase an existing home in an area based on the share of income to mortgage

### Median Household Income

### Rent-Own Ratio
- **Meaning**
  - Another metric to measure house affordability
    - High rent-own ratio means lower house affordability

### Wildfire Hazard Potential (WHP)
- **Meaning**
  - A measurement of the multi-year average of wildfire of a given census tract
    - High WHP means high wildfire risk

### Wildfire Risk to Homes
- **Meaning**
  - A measure that integrates wildfire likelihood and intensity with generalized consequences to a home

## What do features tell us?

### Significantly increased census tracts are also ethnically diverse
- Among all census tracts with a significant population increase, those with a percent of population growth greater than 50% during the past 10 years all have a relatively high diversity index (> 40), indicating
  - Increase of population increase in this region may be driven by an influx of ethnically diverse population in California
  - Combining its relationship with house affordability index, such influx may be caused by more affordable home prices in this region

![image](https://github.com/jiashenyue/ca-wui-pop-increase/blob/main/percent_diversity_index.png)

### Such trend may be driven by home affordability

- A highly diversed census tract tend to have a much lower median home value
![image](https://github.com/jiashenyue/ca-wui-pop-increase/blob/main/diversity_index_med_home_value.png)

- More ethnically diverse census tracts with population increase may have a lower per capita income, restricting the areas to purchase a home

![image](https://github.com/jiashenyue/ca-wui-pop-increase/blob/main/diversity_index_per_capita_income.png)

## Model performance

- Our current model cannot successfully estimate the population increasing rate inside California's high-risk wildfire zone
- The current model and features may work better for census tracts that have an exceptionally high percent of population increase during the past 10 years, rather than all census tracts that have observed a slight population increase
- Future improvements
  - Test if the model performance will be better when the data is further filtered to tracts with exceptionally high percent population increase (e.g. > 10%)
  - Adding features based on geographical location (e.g. county names)
