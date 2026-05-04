## Optimizing Advertising Spend to Maximize Unit Sales
## Executive Summary
This project analyzes how advertising budgets across TV, radio, and newspaper channels influence product unit sales. Using a dataset of 200 observations, I engineered new features, explored spending patterns, and built predictive models to understand which channels drive the strongest sales impact. After comparing Linear Regression, Decision Tree, and Random Forest models, the Random Forest Regressor emerged as the most accurate, achieving an R² of 0.981 and an MAE of 0.620.

The analysis shows that TV advertising is the most influential long‑term driver of sales, while radio provides the highest short‑term lift per $10,000 spent. Newspaper advertising consistently shows minimal impact. These insights help businesses allocate budgets more effectively by identifying which channels generate the highest return on investment.

## Questions for this Project
 * Which advertising channel (TV, radio, or newspaper) has the strongest measurable impact on unit sales, and how should an advertising budget be distributed to maximize sales performance?

* What is the predicted number of units sold based on ad spend by channel level (high/medium/low)?

* What is the marginal increase in units sold for every $10,000 spent?

* Which channel has the most influence on volume?

## Why This Matters
Companies invest heavily in advertising without always knowing which channels actually drive unit sales. Understanding which channels produce the highest return helps businesses avoid wasted spending and improve marketing efficiency.

## Dataset
My dataset's name is Advertising Sales Dataset. I found this dataset on Kaggle, and it is a CSV file.

## Cleaned Dataset
I created a cleaned dataset called f_clean_advertising.csv, which includes:

* Renamed “Sales ($)” to Sales (Units)

* Added new engineered columns

* Removed unnecessary index columns

* Rounded values for consistency

## Link
https://www.kaggle.com/datasets/yasserh/advertising-sales-dataset

## Dataset Information
* 200 rows

* 4 columns

* Little to no cleaning needed

* Minor renaming and formatting changes

* Combined the three ad budget columns to create a Total_Ad_Budget column

## Key Variables I Expect to Use
* TV Ad Budget – spending on TV advertising

* Radio Ad Budget – spending on radio advertising

* Newspaper Ad Budget – spending on newspaper advertising

* Sales (Units Sold) – dependent variable

## Potential Risks
1. Outliers may distort model estimates

2. Extreme ad budgets could skew predictions

3. Some relationships may not be perfectly linear

## Feature Engineering
Several new variables were created to improve the analysis, including:

* Total advertising budget across all channels

* Sales per dollar of advertising spend

* Advertising spend levels (low, medium, high) for each channel

Spend levels were created using quantile binning to categorize budgets into three equal groups. This allows the analysis to examine how different spending tiers impact sales performance.

## Exploratory Analysis
Scatter plots showed:

1. TV advertising has the strongest relationship with sales

2. Radio has a moderate relationship

3. Newspaper has the weakest relationship

These patterns helped guide the modeling approach.

## Analysis and Comparison
   ## Progress Update:

* Added Decision Tree and Random Forest models

* Performed model comparison using R² and MAE

* Identified Random Forest as the best-performing model

* Improved overall model accuracy and insights

## Models Used
 * Linear Regression

* Random Forest Regression

* Decision Tree Regression

## Model Results

## Model	R²	MAE
* Linear Regression	      0.899	1.461
 * Decision Tree Regressor	0.931	0.985
* Random Forest Regressor	0.981	0.620

## Efficiency Results (Sales per Dollar by Spend Level)
TV Spend Level Efficiency
Level	Avg Efficiency
* Low	 0.102306
* Medium	 0.072748
* High	 0.061049


## Radio Spend Level Efficiency
Level	Avg Efficiency
* Low	 0.079763
* Medium	 0.078443
* High	 0.077963


## Newspaper Spend Level Efficiency
Level	Avg Efficiency
* Low	 0.090108
* Medium	0.078013
* High	0.067881


* Interpretation:  
Low spending is the most efficient for all three channels. TV efficiency drops the fastest as spending increases, while radio remains stable across all levels.

## Feature Importance (Random Forest)
Channel	Importance Score
* TV Ad Budget	 0.624810
* Radio Ad Budget	 0.362201
* Newspaper Ad Budget	0.012989


## Permutation Importance
Channel	Importance Score
* TV Ad Budget	 1.486394
* Radio Ad Budget	 0.542192
* Newspaper Ad Budget	0.000059


Interpretation:  
Both methods confirm that TV dominates long‑term influence, radio is secondary, and newspaper has almost no measurable impact.


## Overview of Exploratory and Comparison Analysis

* TV advertising is the most influential predictor of sales

* Newspaper advertising has the weakest impact

* More complex models (Decision Tree, Random Forest) outperform Linear Regression

* Random Forest provides the most consistent and reliable predictions

* TV advertising is also the most important ad

* the most efficent way to go for all three ads was to spend low

## Importance Measurements

TV is the most important channel for long‑term sales growth

Radio provides the strongest short‑term boost

Newspaper has minimal influence and should not be prioritized

## Final Conclusion
Based on the full analysis, several clear conclusions emerge:

TV advertising should receive the largest share of the budget.  
It has the highest feature importance score and the strongest long‑term relationship with sales.

Radio is the best channel for short‑term boosts.  
It delivers the highest marginal increase in units sold per $10,000 spent.

Newspaper advertising provides very little return.  
Both feature importance and marginal gains show that newspaper spending contributes almost nothing to sales performance.

Random Forest is the most reliable model for prediction.  
Its accuracy and low error rate make it the best tool for forecasting sales based on advertising budgets.

Overall, companies should prioritize TV for sustained growth, use radio strategically for rapid lift, and minimize or eliminate newspaper spending.

## What I Learned
Throughout this project, I learned several important lessons:

Feature engineering dramatically improves insights.  
Creating Total_Ad_Budget, channel share percentages, and Sales_per_Dollar revealed patterns not visible in the raw dataset.

Model comparison matters.  
Random Forest captured nonlinear relationships and produced far more accurate predictions than Linear Regression.

Short‑term vs. long‑term impact is different.  
Radio is extremely powerful for quick boosts, while TV dominates long‑term influence.

Visualization makes patterns obvious.  
Scatterplots and bar charts made it clear which channels were strong predictors.

Business context is essential.  
Understanding why a channel performs well helped translate the data into actionable recommendations.

This project strengthened my skills in data cleaning, feature engineering, machine learning, and business‑focused storytelling.


 
