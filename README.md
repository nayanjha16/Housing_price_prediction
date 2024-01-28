# Housing_price_prediction
# House Price Prediction Notebook

## Description
This Jupyter notebook is part of a machine learning project aimed at predicting house prices. It includes a series of regression models, data pre-processing, feature engineering, model evaluation, and validation techniques to ensure the accuracy of the predictions.

## Models Included
- Linear Regression
- Polynomial Regression
- Decision Tree Regression
- Random Forest Regression
- Support Vector Regression
- Gradient Boosting Regression
- XGBoost Regression
- Lasso Regression
- Ridge Regression
- ElasticNet Regression
  
Note:The rationale behind choosing these models and the results obtained with them are present in the notebook.
## Execution

To run this notebook, you must have Python installed on your system, along with the Jupyter Notebook application and several Python libraries such as pandas, numpy, scikit-learn, and matplotlib.

1. Clone this repository to your local machine using:
   git clone [https://github.com/your-username/house-price-prediction.git](https://github.com/nayanjha16/Housing_price_prediction.git)
   

## Evaluation Metrics

The following evaluation metrics are used for evaluating the model performance:
A) Mean Squared Error
B) R-Squared

# Reasons behind choosing Mean Squared Error:  
1) MSE measures the average squared difference between the observed actual outcomes and the outcomes predicted by the model. It directly quantifies how much the regression line deviates from the actual data points.
2) The squaring of the errors in MSE means that larger errors are given disproportionately more weight than smaller ones. This property makes MSE very useful in detecting models that are prone to large errors.
3) MSE is differentiable, this it can be used efficiently during optimization.

# Reasons behind choosing R-Squared:  
1) R-squared measures the proportion of the variance in the dependent variable that is predictable from the independent variables, thus indicating how well the model fits the data.
2) R-squared has a bounded range and thus it improves the interpretability of the results obtained.

