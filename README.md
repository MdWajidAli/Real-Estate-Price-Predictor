# Real-Estate-Price-Predictor


A Machine Learning Project : Real Estate Price Predictor made using Python and its libraries : Panda ,Numpy, Scikit Learn, and IDE : Jupyter Notebook

![Installing libraries](https://user-images.githubusercontent.com/106772487/191845368-78653348-4de7-45c0-94bf-480d7f1b8b38.png)



I started with importing pandas ,imported dataset excel sheet to a variable housing, accessed different attributes from the dataset and checked their counts.



### Important steps as we start with the project :

## 1. Train-Test Spitting :

   The train-test split is used to estimate the performance of machine learning algorithms that are applicable for prediction-based Algorithms/Applications. This method is a fast and easy procedure to perform such that we can compare our own machine learning model results to machine results.
By default, the Test set is split into 30 % of actual data and the training set is split into 70% of the actual data.

Syntax :

	train_test_split(*arrays, test_size=None, train_size=None, random_state=None, shuffle=True, stratify=None)
	

![Train and Test data splittin](https://user-images.githubusercontent.com/106772487/191845811-84c75768-8bff-4055-b97a-72a0110acf5c.png)




## 2. Looking for Coorrelations :
Correlation can be an important tool for feature engineering in building machine learning models. Predictors which are uncorrelated with the objective variable are probably good candidates to trim from the model (shoe size is not a useful predictor for salary). In addition, if two predictors are strongly correlated to each other, then we only need to use one of them (in predicting salary, there is no need to use both age in years, and age in months). Taking these steps means that the resulting model will be simpler, and simpler models are easier to interpret.

There are many measures for correlation, but by far the most widely used one is Pearson’s Product-Moment coefficient, or Pearson’s r. Given a collection of paired (x,y) values, Pearson’s coefficient produces a value between -1 and +1 to quantify the strength of dependence between the variables x and y. A value of +1 means that all the (x,y) points lie exactly on a line with positive slope, and inversely, a value of -1 means that all of the points lie exactly on a line with negative slope. A Pearson’s coefficient of 0 means that there is no relationship between the two variables.

## 3. Trying out Attribute Combinations :
Attribute subset Selection is a technique which is used for data reduction.Attribute subset Selection is a technique which is used for data reduction.

The data set may have a large number of attributes. But some of those attributes can be irrelevant or redundant. The goal of attribute subset selection is to find a minimum set of attributes such that dropping of those irrelevant attributes does not much affect the utility of data and the cost of data analysis could be reduced. Mining on a reduced data set also makes the discovered pattern easier to understand.

-Methods of Attribute Subset Selection-

- Stepwise Forward Selection.
- Stepwise Backward Elimination.
- Combination of Forward Selection and Backward Elimination.
- Decision Tree Induction.

## 4.Scikit-Learn Design :
Scikit-Learn. Scikit-Learn is a powerful, rich, and extensive Python library for implementing machine learning. The library provides tools for modeling (e.g., classification, regression, and clustering algorithms), model selection (e.g., grid search), preprocessing (e.g., feature extraction), and more. I maintain that the success of the library has as much to do with its interface and ease of use, as it does with its powerful and profound functionality.

-Primarily , three types of objects
- Estimators
- Transformers
- Predictors

## 5.Feature Scaling :
Primarily, 2 types of feature scaling methods:

Min-max scaling (normalization)
(value-min)/(max-min)
sklearn provides a class called MinMaxScaler for this

Standardization
(value - mean)/std
sklearn provides a class called standard scaler for this

## 6.Creating a Pipeline :
A Machine Learning pipeline is a process of automating the workflow of a complete machine learning task. It can be done by enabling a sequence of data to be transformed and correlated together in a model that can be analyzed to get the output. A typical pipeline includes raw data input, features, outputs, model parameters, ML models, and Predictions. Moreover, an ML Pipeline contains multiple sequential steps that perform everything ranging from data extraction and pre-processing to model training and deployment in Machine learning in a modular approach. It means that in the pipeline, each step is designed as an independent module, and all these modules are tied together to get the final result.

## 7.Selecting the desired model :
Having a wealth of options is good, but deciding on which model to implement in production is crucial. Though we have a number of performance metrics to evaluate a model, it’s not wise to implement every algorithm for every problem. This requires a lot of time and a lot of work. So it’s important to know how to select the right algorithm for a particular task.

## 8.Cross Validation :
It is a technique in which we train our model using the subset of the data-set and then evaluate using the complementary subset of the data-set.

The three steps involved in cross-validation are as follows :

1.Reserve some portion of sample data-set.
2.Using the rest data-set train the model.
3.Test the model using the reserve portion of the data-set.

## 9.Decision Tree Classification :
Decision Tree is a Supervised learning technique that can be used for both classification and Regression problems, but mostly it is preferred for solving Classification problems. It is a tree-structured classifier, where internal nodes represent the features of a dataset, branches represent the decision rules and each leaf node represents the outcome.

In a Decision tree, there are two nodes, which are the Decision Node and Leaf Node. Decision nodes are used to make any decision and have multiple branches, whereas Leaf nodes are the output of those decisions and do not contain any further branches

It is a graphical representation for getting all the possible solutions to a problem/decision based on given conditions.

## 10.Testing the model :
Testing identifies explicitly which part of the code fails and provides a relatively coherent coverage measure (e.g., lines of code covered). It helps us in two ways:

Quality assurance; whether the software works according to requirements, and
Identify defects and flaws during development and in production.
