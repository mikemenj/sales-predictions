# Recommendation of Regression Tree Model for sales predictions
## Comparison of performance of Linear Regression Model  vs Regression Tree Model

**Author**: Michael Menjares

### Business problem:

Which of the two models would be best for predicting sales given a set of features?

### Data:
Link to Data: https://drive.google.com/file/d/1syH81TVrbBsdymLT_jl2JIf6IjPXtSQw/view

Original Data Source from Analytics Vidhya: https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/

There were 8523 rows and 12 columns for this dataset

<p align = "center"> 
  <img src = "https://github.com/mikemenj/sales-predictions/blob/main/data%20dict.png">
</p>

## Methods
###Exploratory Data Analysis

- Data preparation steps with explanation and justification for choices
- 

## Results
#### Linear Regression Scores
![Linear Regression Scores](linreg%20scores.png)
> R2 Scores on Linear Regression could be improved but does show low variance

#### Visualizing which max_depth leads to the highest r2 score
![Max Depth](max%20depth.png)
> A max depth of 5 provided the best R2 score.

![Reg Tree Metrics](reg%20tree%20metrics.png)
> After tuning for max depth, R2 score increased
> 
## Model

Regression Tree model did perform better than linear regression but even after tuning it wouldnt be reliable since it had an R2 score of 59.5 and was off by 1057 for RMSE

## Recommendations:

If had to choose between the two, i would recommend the Regression Tree model but it still wouldnt be a reliable predictor of sales since still has bias.

## For Further Information
 For additional question, please contact me on LinkedIn: https://www.linkedin.com/in/michael-menjares/
