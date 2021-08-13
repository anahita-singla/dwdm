# dwdm
The objective of the dataset is to diagnostically predict whether or not a patient has diabetes, based on certain diagnostic measurements included in the dataset.
The datasets consists of several medical predictor variables and one target variable, Outcome. Predictor variables includes the number of pregnancies the patient has had, their BMI, insulin level, age, and so on.



## k-Nearest Neighbor 
KNN is a supervised classification algorithm, note — a supervised algorithm uses training data whereas an unsupervised algorithm has no training data.
If we use KNN to solve this problem and set k = 5 the algorithm will look for the five closest data points to the red dot using EUCLIDEAN DISTANCE MEASURE.

Steps: We split our data into training data and test data. 
Calculated euclidean distance for each training data with each test data (n^2). (pick 1 testdata and find dist from entire training data)
Sorted our results based on distance of each training data from test and chose K NEAREST NEIGHBOUR. 
if K nearest neighbours are +ve- our result from classification is +ve. 
if the given outcome from euclidean distance is near to test distance measure according to +ve and -ve classes, they were put under true +ve and true -ve respectively. Otherwise false +ve and false -ev.

After calculating same for all test data, final accuracy is calculated as (truePositive + trueNegative) / (truePositive + trueNegative + falsePositive + falseNegative))*100


## NAIVE BAYES
Naive Bayes is a classification algorithm, which uses Bayes theorem of probability for prediction of unknown class. 
It uses probability to decide which class a test point belongs to. Naive Bayes is a purely statistical model. 
This algorithm is called Naive due to the assumption that the features/ attributes in the datasets are mutually independent.
Type of naive bayes model:Gaussian: It is used in classification and it assumes that features follow a normal distribution(continuous values)
steps: We split our data into training data and test data. 
probability is calculated according to following gaussian naive bayes formula. 
Prepared the summary of each class by using mean and standard deviation of each attribute/column.
![alt text](https://d1zx6djv3kb1v7.cloudfront.net/wp-content/media/2019/11/Gaussian-Naive-Bayes-i2tutorials.jpg)
