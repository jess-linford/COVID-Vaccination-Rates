# COVID-Vaccination-Rates
Predicting COVID vaccination rates by county from demographic and political data

This was a project for STAT 656 - Applied Analytics at Texas A&M. Our goal was to determine what factors are most important in predicting a county's vaccination rate and create a model to predict vaccination rates from demographic and political data. 

We used demographic data from the US Census Bureau, 2020 election data from the New York Times, and COVID data from the CDC and state departments of public health. We centered and scaled our features and performed a Yeo-Johnson skewness correction on highly skewed features.

We tested several models on a group of hand-selected variables and on a list of variables created by correlation filtering. Our best model (as determined by lowest test error) turned out to be an elastic net model on the correlation-filtered data. We also attempted basic multiple linear regression, boosting, and refitted lasso models. Attempts to use Poisson regression with an offset term and random forest models are not shown in this file.

In every model we tested, the percent of voters in the county who voted for Joe Biden in the 2020 election was the most important predictor. This factor had a strong positive correlation with vaccination rate. In most of our models, the proportion of county residents who are Black was the 2nd most important predictor. This factor had a moderate negative correlation with vaccination rate.

A Google Slides presentation of our project can be found here: https://docs.google.com/presentation/d/1ogi6OKBLyfyAWzORbZcu7blPUjEamcsmBFxrJTLV3zc/edit?usp=sharing
