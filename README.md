# Predicting the annual medical expenses (in dollars) of a person to set insurance premium, greater than the predicted medical expenses for earning profit. 
Used 5 regression algorithms, linear regression, polynomial regression, ridge regression, xgboost regression and neural network regression to find the best ML model to predict medical expenses of a person on the basis of features like age, sex, bmi, region, children, smoker.
Data was taken from the Kaggle website. The data set contains various attributes of 1338 individuals including the total amount of medical expense incurred for one year. The attributes for this data set is shown below:
### • Medical Charges: Total medical expense charged to the plan for the calendar year
### • Age: Insurance contractor’s age, ranging from 18 to 64
### • Sex: Insurance contractor’s gender, Male or Female
### • BMI (Body Mass Index) = Body Mass Index, Weight(Kg)/( Height(m)² )
### • Children: Number of children covered by the plan/ Number of dependants
### • Region: The beneficiary’s residential area in the US. Northeast, Southeast, Northwest, Southwest
### • Smoker: Whether the insurance contractor is a smoker or not, Yes or No
As mentioned, medical charges will be our dependent variable and the rest will be our independent variables.


 After extensive exploratory data analysis, came to the conclusion, that people having smoking habit have very large medical expenses and this feature is very highly correlated with the medical expenses.
 Also, the more the bmi,age the unhealthier the person, the higher the medical expenses. Using Anova test, found out that the region is an insignificant feature for using in model, so dropped it. Males have higher
 average medical expenses than females and medium sized families (2-3) children have higher medical expenses than small(0-1 children) and large(4-5 children). Created 
 the 5 regression models,optimized them, by trying to enhance their r2_score and root mean square error, on the basis of which these algorithms were judged. 
## On the basis of the avove analysis, came to the following conlusion:

# THE MODELS, ARRANGED ACCORDING TO BEST R2 SCORE AND LEAST ROOT MEAN SQUARE ERROR ON TEST SET IS:

### 1. XGBOOST REGRESSOR (R2_SCORE:0.8989763016162411, RMSE:3770.9750251931814)


### 2. POLYNOMIAL REGRESSION (R2_SCORE:0.8873703433315301, RMSE:3981.698801889921)


### 3. NEURAL NETWORK REGRESSION (R2_SCORE: 0.8789103065028973, RMSE:4128.531611673513)


### 4. RIDGE REGRESSION (R2_SCORE: 0.8784750985619123, RMSE:4135.944126084564)


### 5 .LINEAR REGRESSION (R2_SCORE: 0.7867465671074685, RMSE:5478.857939886519) 

