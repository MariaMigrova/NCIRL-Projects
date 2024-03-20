# NCIRL-Projects
## 1. Project Title: Multiple Linear Regression
### Introduction
Predictive modeling, also known as predictive analysis, involves forecasting future events or outcomes by examining patterns from historical data. The main objective is to predict future results based on past behavior. This approach finds applications in various fields such as weather forecasting, customer behavior analysis, and pricing strategies. The process of predictive modeling involves determining the appropriate model family and fitting the model to the data.

### Regression
Regression is a statistical technique used to determine the strength and nature of the relationship between a dependent variable and a set of independent variables. It finds extensive use in industries like banking and investment.

### Simple Linear Regression
Simple linear regression models the dependence of a response variable on a single explanatory variable. It assumes a straight-line relationship between the two variables, with the intercept representing the expected mean value of the response variable when the explanatory variable is zero, and the slope indicating the change in the response variable for a unit change in the explanatory variable. The goal is to find the line of best fit that minimizes the squared errors between the observed and predicted values.

### Methodology
#### Data Description
The project utilizes a dataset called Credit_v2.csv containing nine variables and 687 observations. These variables include age, education level, years with current employer, years at current address, household income, debt to income ratio, other debt, default status, and credit debt amount. After summarizing the data and examining outliers, we proceed with model building.

#### Building the Model
The project aims to predict credit debt using other dependent variables. We compare different linear models for various independent variables and select the model with the highest R-squared value. After trying different combinations of variables, we finalize a model including employment duration, income, debt to income ratio, and other debt. Surprisingly, a model using the " * " operator instead of " + " results in a perfect fit.

#### Plotting the Results
We visualize the predicted credit debt using linear models and plot the residuals to assess model performance. The second model, with the " * " operator, exhibits nearly perfect predictions, while the first model shows some deviation.

### Assumptions
Assumption tests reveal issues with linearity, normality, and homoskedasticity in the first model, necessitating transformation of the response variable. The second model meets most assumptions.

### Data Accuracy Metrics
We evaluate model performance using Mean Absolute Error (MAE), Mean Absolute Percentage Error (MAPE), and Mean Squared Error (MSE) metrics. Both models perform well, but the second model outperforms the first significantly.

## 2. Project Title: Time Series and Logistic Regression
### Introduction to Time Series
Defined time series as data collected over time, with components including trend, cyclical effect, seasonal variation, and residual effect.

### Forecasting Methods:
Mean Forecast Method: Using the average of the time series to predict future values.
Naive Method: Forecasting future values based on the value of the previous period.
Seasonal Naive Method: Modifying the Naive Method for highly seasonal data.
ARIMA Method: Auto-Regressive Integrated Moving Average method for time series forecasting.

### Model Evaluation:
Calculated forecast accuracies using Mean Absolute Percentage Error (MAPE) and Root Mean Squared Error (RMSE).
Evaluated each forecasting method's performance based on RMSE and MAPE values.

### Conclusion and Future Work:
Identified the Naive Method as the best-performing forecasting model.
Suggested future work including exploring more complex time series forecasting models like SARIMA, XGBoost, or LSTM algorithms.

### Logistic Regression Analysis:
#### Introduction to Logistic Regression
Defined logistic regression as a method for predicting a categorical dependent variable based on independent factors.

#### Assumptions of Logistic Regression:
Dependent variable must be categorical.
No multicollinearity in independent variables.
Independence of errors.
Linearity in the logit for continuous variables.

#### Model Building and Evaluation:
Created logistic regression models using glm() function in R.
Evaluated model coefficients, AIC values, and performed Confusion Matrix analysis.

#### Conclusion and Future Work:
Found the second logistic regression model slightly outperformed the first one.
Suggested potential improvements such as normalizing data, addressing class imbalance, hyperparameter tuning, exploring more classifiers, or conducting error analysis.
