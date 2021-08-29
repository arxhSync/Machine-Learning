
# Wine Quality Model

Here I made Machine learning model where I am using Random Forest algorithm. So we have to check the quality of wine and score it 0 to 10.
So, I get this data from kaggle and there are 11 independent variable and 1 is dependent variable (Quality) or target variable.

## About Random Forest
Random forest algorithm is a supervised classification algorithm

The random forest is a classification algorithm consisting of many decisions
trees.

It uses bagging and feature randomness when building each individual tree to
try to create an uncorrelated forest of trees whose prediction by committee is
more accurate than that of any individual tree

Higher the number of trees in the forest gives the high accuracy results.

### For Classification

Calculate the votes for each predicted target.

Consider the high voted predicted target as the final prediction from the
random forest algorithm.

his concept of voting is known as majority voting.

## Data cleansing 

There are some null values and duplicate values in the data. So, i just replace it with the Mean value of a particular column.
We also adjusted the outliers after checking boxplot 

## Model Architechture

First I imported various Python library like NumPy, Pandas.
And for visualization Matplotlib and seaborn.

After checking that is there any null and duplicate values or not. I started EDA, built various pie chart, Bar plot, heatmap for checking correalation amoung the variables, boxplot.

So there are many insights came to see while performing EDA like - 
- Using box plot, we are showing outliers in all the independent variable using for loop.
- we check value counts on Grade and quality column
- Composition of chloride also go down as we go higher in the quality of the wine
- we showed correalation amoung all the variables using heat map and in dataframe.
- plotted boxplot before and after treating outliers

## Deploying Model

So now we imported sklearn library. And from sklearn we imported Random Forest classifier.
imported min max scaler , train test split, accuracy score

We divided data set into train and test. In training set 80% of the data and in testing set 20% of the data.
Here we also add random state=41 so, every time data will be same.

- we used randomized grid search 
randomized Gridsearch cv = will not run all the combinations, will pic parameter values at random and train the model with them

Grid Search CV helps to find best set of parameters by training the algorithm and seeing the results
clf = RandomForestClassifier() # defining Classifier


Fitting the decision tree classifier on both x_train and y_train data and predicting the model on Test data

here we have to choose the depth of the trees and the estimators and sample leaf.

At last we caculated our accuracy which is very good 73%.




