
# Dengue Fever Case Prediction

A comprehensive study where 2 friends and I compared the effectiveness of 3 AI models in predicting weekly Dengue Fever cases in the cities of San Juan, Puerto Rico and Iquitos, Peru. The 3 models used were Support Vector Machines, Random Forest and Lasso Regression. This project was done for my Data Science with Machine Learning module during my Master's. The accompanying .pdf file is our full report that explains the scientific logic behind our results. The data and the task used in this study comes from the DengAI DrivenData competition and can be found at: https://www.drivendata.org/competitions/44/dengai-predicting-disease-spread/
## Important Disclaimer

Since this notebook was developed for one of my projects during my Master's, it needed to have a scientific aspect. That's why we trained 3 different models. We also wanted to see the effect of using less features on the performance, so for each model, we trained one version with 6 features, and one version with 10 features. Hence, this notebook trains and evaluates 6 models. Moreover, we did bayesian optimization and Grid Search for hyperparameter tuning, where we did several trials with different parameter grids for each model and each feature space. In addititon, there are many complex plots, and nested cross-valdation. 

Moral of the story is, the code can and will take HOURS to run. If you are trying to run it, please comment out the unneccessary bits that you don't need to see, otherwise it will take forever. If this was just for the competition and wasn't a scientific research project, we would have not added a great majority of these steps and the code would be much shorter and would run much faster. If you would like to skip ahead and just see the results, you can check our .pdf report.

## Table of Contents

- [Objective](#objective)
- [Abstract](#abstract)
- [Credits](#credits)

## Objective

The objective of this study was to see the performance of 3 different ML models in predicting weekly Dengue cases. To do so, we used SVM, Random Forest and Lasso Regression. We also re-ran the experiments with 6 and 10 features to see the difference. The features are related to humidity, temperature and weather conditions in general. 
## Abstract

Dengue is an endemic tropical disease spread by Aedes aegypti mosquitoes. This study attempted to model and understand dengue spread in two cities San Juan, Puerto Rico and Iquitos, Peru. It attempted to understand and predict the weekly dengue cases and dengue outbreaks in the city by comparing the Random Forest Regression, Support Vector Regression and Lasso Regression. The study used Bayesian hyperparameter optimization and tried to understand the effect of changing the scoring metric for the hyperparameter optimization algorithm from mean absolute error to coefficient of determination and its effect on the predictive ability of the produced models. Finally, it also used a feature importance analysis to extract the most important features and attempted to understand the effect of increasing the number of features (from 6 features to 10 features) and its effect on the predictive ability of the models. The results were analysed using various average performance metrics ( Mean absolute error (MAE), root mean squared error (RMSE) and coefficient of determination (R2)) obtained through the nested cross-validation methodology and confidence intervals were provided for these metrics. 

For the city of San Juan the Support Vector Regression produced more promising performance metrics but the random forests model was able to predict dengue outbreaks with a much greater degree of accuracy. In general, for both cities changing the scoring metric to R2 the hyperparameter optimization diminished the performance metrics of the models that had performed well under the MAE scoring metric and did not in general affect or improve any of the remaining models. A similar result was obtained when the number of features used to create the machine learning model was increased from 6 to 10.
## Credits

This project was done as a group effort with my friends Sundeep and Hassan. I mainly focused on the Random Forest Regressor, while Sundeep focused on the Support Vector Regressor and Hassan worked on the Lasso regression. The data analysis was a combined effort and we wrote the paper together. Their contact details can be found on our report.
