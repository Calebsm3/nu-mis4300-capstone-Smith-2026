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

## Exploratory Analysis

Scatter plots showed:

* TV advertising has the strongest relationship with sales
  
* Radio has a moderate relationship
  
* Newspaper has the weakest relationship
  
## Analysis and comparison

Progress Update

* Added Decision Tree and Random Forest models
* Performed model comparison using R² and MAE
* Identified Random Forest as the best-performing model
* Improved overall model accuracy and insights

for this section, I first made a comparison for all 3 advirtising columns and compared them to sales. I then went and made three models to see which one is the most accurate and which one has the least amount of mistakes.
the three models I used where:
* Linear Regression

* Random Forest Regression

* Decision Tree Regression

I then did a comparison of the 3 using R2 and MAE and these where the results were:


* Linear Regression
  
R2: 0.899
MAE: 1.461

* Decision Tree Regressor
  
 R2: 0.931
MAE: 0.985

* Random Forest Regressor
  
R2: 0.981
MAE: 0.620


With this information, I found that the Random forest was both the highest for my R2(accuracy) and the lowest for my MAE(Mistakes)
I then made a bar graph for the R2 and MAE.

## Overview of exploratory and comparison analysis

* TV advertising is the most influential predictor of sales
  
* Newspaper advertising has the weakest impact
  
* More complex models (Decision Tree, Random Forest) outperform Linear Regression
  
* Random Forest provides the most consistent and reliable predictions


## Importance measurements

 * I found that the most important ad to spend money on was Tv by far especially in the long run
 * I also found that the most important for a short term boost is the radio
 * newspaper was pretty low and should not be used near the other 2


 
