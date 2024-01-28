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


## Inferences:
Generally, the models with complex learning objective for e.g: xg Boost tend to perform better than simpler models such as linear regression. However in this case we find the right opposite, The linear regression model performs the best among the other models whereas XG Boost has the highest MSE loss.

 This could be due to the following factors:

1) The association between the data is simpler hence more complex models overfit.

2) The size of the training data is only 800 records, which is quite small. This could be another reason behind such results.

3) It is observed that the Decision tree performs the worst but the Random forest performs better. This is another example where the ensemble technique improves the performance.

4) The same trend of MSE is reflected in R-squared loss.

5) Looking at the individual plots for the predicted values of the training and testing data, we can conclude the following:

5A) Models like Decision Tree Regressor and xg Boost seem to overfit as they perform well on the train set data when the prediction is made but the same on test set is quite poor.

5B) Models like Support Vector Regression, Lasso Regression, Ridge Regression, and Elastic Net Regression seem to underfit as we see that for the predicted values of train set too, there is a huge variance between the actual training points and the predicted training points. This implies that the learning for the aforementioned models was poor.

## Scope of Improvement:

1) Since the data is less, increasing the training data should help us overcome overfitting.

2) Hyperparameter tuning can help us improve the accuracies further.

3) Sticking to simpler architectures due to a lack of training data is another solution that can be implemented.

4) We can try doing feature selection, in an iterative manner to understand if by eliminating some features model accuracy can be improved further.

5) For the underfitting models we can try running it for more iterations to see if that helps the model learn.
