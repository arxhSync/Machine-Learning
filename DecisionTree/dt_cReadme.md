
# University Admission Model

Here I made Machine learning model where I am using Decision tree algorithm. Whether the University going to admit the candidate or not. 
So, I get this data from kaggle and there are 8 independent variable and 1 is dependent variable or target variable.

A decision tree is built top-down from a root node

### Root Node:
It represents entire population or sample and this further gets
divided into two or more homogeneous sets.

### Splitting: 
It is a process of dividing a node into two or more sub-nodes.

### Decision Node: 
When a sub-node splits into further sub-nodes, then it is called
decision node.

### Leaf/ Terminal Node: 
Nodes with no children (no further split) is called Leaf or
Terminal node.

### Branch / Sub-Tree:
A sub section of decision tree is called branch or sub-tree.

### Parent and Child Node: 
A node, which is divided into sub-nodes is called parent
node of sub-nodes where as sub-nodes are the child of parent node

## Data cleansing 

There is no null values and duplicate values in the data. So, i just started EDA (Exploratory ata Analysis).

## Model Architechture

First I imported various Python library like NumPy, Pandas.
And for visualization Matplotlib and seaborn.

After checking that is there any null and duplicate values or not. I started EDA, built various Bar plot, heatmap for checking correalation amoung the variables, boxplot.

So there are many insights came to see while performing EDA like - 
- count of students as per there Gre score and CGPA score.
- count of students who did research and who did not.
- Value counts on the basis of University rating.

## Deploying Model

So now we imported sklearn library. And from sklearn we imported decision tree classifier and regressor.
imported min max scaler , train test split, accuracy score

We divided data set into train and test. In training set 80% of the data and in testing set 20% of the data.

then we fit the training and tesing sets using minmaxScaler()

Fitting the decision tree classifier on both train and test data and predicting the model on Test data

At last we caculated our accuracy which is very good 78%.




