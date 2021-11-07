# HousePrices
Predicting sales prices and practice feature engineering, RFs, and gradient boosting


* Lasso regressions performs best with a cross validation RMSE-score of 0.1121. Given the fact that there is a lot of multicolinearity among the variables, this was expected. Lasso does not select a substantial number of the available variables in its model, as it is supposed to do.
* The XGBoost model also performs very well with a cross validation RMSE of 0.1162. 
* As those two algorithms are very different, averaging predictions is likely to improve the predictions. As the Lasso cross validated RMSE is better than XGBoost's CV score, I decided to weight the Lasso results double.
