# random_forest
Random forests provide an improvement over bagged trees by way of a that decorrelates the trees. As in bagging, we build a number of 
decision trees on bootstrapped training samples. But when building these decision trees, each time a split in a tree is considered, 
a random sample of m predictors is chosen as split candidates from the full set of p predictors The split is allowed to use only 
one of those m predictors. A fresh sample of m predictors is taken at each split, the number of predictors considered at each split is 
approximately equal to the square root of the total number of predictors.

In this program we have generated three graphs by selecting subset of the attributes which contain 2 elements so the that there is no 
correlation among the trees.We generated three different graphs for each of the data set by redirecting the output to the dot file.The
output obtained are out1.txt,out2.txt,out3.txt.The graphs hence generated are graph1.png,graph2.png,graph3.png.Once the model is generated 
we use a set of featues to predict the class label.In the present modelthe features used in the prediction of the class is 
body temperature-1(warm),gives birth-1(yes),aquatic-0(no),aerial-0(no),has legs-1(yes),hibernates-0(no).The result obtained by each of 
the model is written to the file result1.txt,result2.txt and result3.txt respectively and later they are combined to a single file 
result.txt.

In random forest if it is a regression model then the result of prediction would be the average of the values obtained by the predictive 
models,but in classsification model majority vote is considered.

By clear observation we can make out that the class predicted by three models is "mammal".So the class of the data point which was given to
predict is "mammal".

Therefore with the help of random forest we can arrive at a most accurate result.
