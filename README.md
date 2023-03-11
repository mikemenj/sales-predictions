# Recommendation of Tuned Regression Tree Model for sales predictions
## Comparison of performance of Linear Regression Model  vs Regression Tree Model vs Tuned Regression Tree Model

**Author**: Michael Menjares

### Purpose:

The purpose of this analysis is to compare the performance of a Linear Regression model and a Regression Tree model in predicting sales, and recommend which model would be the best choice based on their respective strengths and weaknesses.

### Data:
Link to Data: https://drive.google.com/file/d/1syH81TVrbBsdymLT_jl2JIf6IjPXtSQw/view

Original Data Source from Analytics Vidhya: https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/

There were 8523 observations and 12 variables for this dataset

During data preparation, missing values were identified and addressed using SimpleImputer from scikit-learn in the preprocessor pipeline to impute the missing values. Also, the Item_Fat_Content column had inconsistencies in labeling. These issues were addressed by using the replace() function from pandas to merge similar values.

<p align = "center"> 
  <img src = "https://github.com/mikemenj/sales-predictions/blob/main/data%20dict.png">
</p>

### Methods:
To prepare this data, the data was cleaned, and the following processes were performed:
Exploratory Data Analysis
- During the exploratory data analysis, a bar chart was visualized to show the distribution of the categorical variables Item_Fat_Content, Item_Type, and Outlet_Size.
  Supermarket Type 3 made the most sales on average, followed by Supermarket Type 1.
- Also, a bar chart was used for the sales by each Item Type. Household items was the most sold Item Type follow by Fruits and Vegetables.
Maching Learning Using the Following Models:
- Linear Regression
- Decision Tree Regressor Model
- Tuned Decision Tree Regressor Model

## Models Evaluated & Results

- Linear Regression Model (Testing Set):
  - R^2: 0.567725	
  - MAE: 802.7744	
  - RMSE: 1092.0797

- Decision Tree Regressor Model (Testing Set):
  - R^2: 0.195271
  - MAE: 41512.219
  - RMSE: 61723.863

- Tuned Decision Tree Regressor Model (Testing Set):
  - R^2: 0.59471
  - MAE: 738.3173
  - RMSE: 1057.4431

The Final Model Chosen was the Tuned Decision Tree Regressor Model with the n_estimators tuned to 5.

For the testing set on the model, 59.5% of the variance in y was explained by x.

The Mean Absolute Error was off by about 738 sales.

The Root Mean Squared Error had a calculation of 1057 sales.

## Recommendations:

Out of the three models, I would recommend the Tuned Regression Tree model but it still wouldn't be a reliable predictor of sales.

## For Further Information
 For additional question, please contact me on LinkedIn: https://www.linkedin.com/in/michael-menjares/
