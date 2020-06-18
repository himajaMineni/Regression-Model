# Regression-Model
Predicting the Mosquito virus using Machine Learning Regression Model

Dataset Description:
 To perform this I used logistic regression as my target variable is having two labels positive or negative. This dataset contains 12 attributes excluding the target variable, and there are 29489 rows in the dataset. For the analysis logistic regression algorithm to predict the results, to implement this algorithm I first imported the package name pandas to read my CSV file. 
 
 
Regression Analysis:
Regression analysis is a best-suited model for prediction analysis, and it is also a statistical model that gives the relation of one variable with the other. It shows how a dependent variable changes with an independent variable. There are many types of regression analysis, they are, linear regression, logistics, regression, quantile regression, etc. regression analysis is widely used for prediction analysis and forecasting. The most popular type of regression analysis is the linear model, it gives the linear relation between the variables and next to it is the logistic regression analysis.


Logistic Regression:
Logistic is a statistical model well used for prediction analysis, we use a logistic function to develop a model for a binary target variable. In general, logistic regression will have two possible outcomes pass or fail, positive or negative, true or false. These outcomes are labeled as 1 or 0, the label 1 indicates the linear combination of independent variables. These independent variables can be either continuous or discrete variables. The logistic function is defined by a sigmoid function and having a threshold of 0.5 so the output varies between 0 and 1. Here the probability of the target variable labeled “1” varies between 0 and 1.


Algorithm implementation:
This data is very clean and well processed as there are no missing values in the dataset, this has made my work a little easier and gave me accurate results. The dataset contains column names with season year, week, test id, block, trap, trap type, number of mosquitoes, result, species, latitude, longitude, location. From these 13 columns, I have dropped a few columns like season year, week, test id, location, latitude, longitude as these columns do not contain any data that is necessary for my prediction analysis.
Here, after dropping a few unnecessary columns I imported the model selection package from sklearn to split the data into the train set and test set. Later I also imported the logistic regression model from the linear model package. By fitting the logistic regression model on my dataset I encountered an error saying string can not be converted into the float. To overcome this error I imported the preprocessing library from the sklearn package and with the use of label encoder function I fit and transform the string into the float. Later I selected the feature variables and the target variable and converted them into data values from the NumPy package that I imported. Then I split the data into the train set and the test set with a ratio of 80:20. Then applied the logistic regression model using the regression function I imported from the sklearn. Next to that, I found the predicted values by using the predict function. Now to check the accuracy of the model I imported the metrics and scorer to check the accuracy which gave an accuracy of 90 percent. 
