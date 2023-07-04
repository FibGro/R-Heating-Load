# Heating Load Prediction 

The project is part of the learning by building the regression model section. The main objective of this project is to implement the regression method that we have been learned in the class. The specific goal of the project is to predict the heating load of residential buildings based on the following characteristics of the building: Relative compactness, Surface Area, Wall Area, Roof Area, Height, Orientation, Glazing Area, and Glazing Area Distribution. The prediction of the heat load is important to ensure energy-saving and improve system operation efficiency. 



# Dataset Information 

The data was created by Angeliki Xifara (Civil/Structural Engineer) and was processed by Athanasios Tsanas (Oxford Centre for Industrial and Applied Mathematics, University of Oxford, UK). The data is collected from analysis utilizing 12 different building shapes simulated in Ecotect. The buildings differ concerning the compactness, the surface area, and the roof area, amongst other variables. The data set contains eight variables and two outcomes, denoted by Y1 and Y2. However, in this project, we only predict one outcome which is heating load (Y1). The link of data can be found in [here](https://archive.ics.uci.edu/ml/datasets/energy+efficiency).

# End Result

The end result can be found in my Rpubs : https://rpubs.com/Fib_Gro/Heating_Load

# File Attachment 

- Rmd file 
- csv file 
- RDS file (Random Forest) 
- Pictures file

# Conclusion

1. Linear regression method has been performed to predict the heating load of the building.
2. Height, wall area, surface area, compactness, glazing area, and glazing distribution have a significant influence on the target variable.
3. The prediction of the heating load by using the linear regression method shows that the model with the stepwise method is a better model than the lm() model due to having the highest value of an adjusted R-squared and the lowest value of error (RMSE).
4. Linear regression method is not the most appropriate method for this dataset because the model violates three assumptions (multicolinearity, normality of residuals and homoscedasticity).
5. The transformation on target and predictor has been done. However, it does not change the violation of the linear regression assumption.
6. We had a total of 4 regression models : linear regression, ridge regression, decision tree and random forest. Random forest is the most appropriate model for predicting heating load with a RMSE of 0.547.
7. The quantile regression model is used to find the relationship between target and predictors that changes depending on which quantile we look at.
8. Only quantile coefficients for height and roof area have differences from the estimated OLS coefficients. While for the other variables, the linear regression coefficient is sufficient to describe the relationship between target and predictor.
