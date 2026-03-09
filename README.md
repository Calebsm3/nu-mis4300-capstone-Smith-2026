## project Title
Optimizing Advertising Spend to Maximize Unit Salesthe primary project 


## Questions for this Project

 * Which advertising channel (TV, radio, or newspaper) has the strongest measurable impact on unit sales, and how should an advertising budget be distributed to maximize sales performance?
    *  what  is the Predicted units sold based on ad spend by channel level(high/medium/low)?
    *   what is the marginal increase in units sold for every $10,000 spent?
    *    which channel has the most influence on volume?
   
## Why This Matters:

this matters becuase a lot of companies put a lot of money into these advirtisements without knowing which one truly drives unit sales.

## Dataset

My dataset's name is advirtising sales Dataset. I found this dataset on Kaggle, and it is a CSV file.

## Cleaned dataset

I made a new cleaned dataset that has changed the name of sales to sales units and has added some new columns for analysis
f_clean_advirtising.csv

## Link

https://www.kaggle.com/datasets/yasserh/advertising-sales-dataset

## Dataset information

* 200 rows
* 4 columns
* Little to No cleaning needed
* changes to the column names and values needed
* combining the three Ad budget columns to make total ad budget columns

## Key Variables I Expect to Use:

I expect to use all four variables in my project, the four being:
 * TV Ad Budget, spending on TV advertising.
 * Radio Ad Budget, spending on radio advertising.
 * Newspaper Ad Budget, spending on newspaper advertising.
 * Sales (Units Sold), product units sold (dependent variable)
   
## Potential Risks

* Some potential risks I could have with this project are Outliers
*  Extreme ad budgets could distort model estimates. 
* some of the data not beign linear with the amount spent.

## Feature Engineering

Several new variables were created to improve the analysis, including:

 * Total advertising budget across all channels

   * Sales per dollar of advertising spend

   * Advertising spend levels (low, medium, high) for each channel

Advertising spend levels were created using quantile binning to categorize budgets into three equal groups. This allows the analysis to examine how different spending tiers impact sales performance
  
## Next steps:

My next few steps is to Clean and explore the dataset (summary statistics, correlations, visualizations), Fit a multiple linear regression model and Evaluate model performance.
