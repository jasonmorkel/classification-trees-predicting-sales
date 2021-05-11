# classification-trees-predicting-sales
Using the tree library to construct a classification tree

Classification tree is first plotted to analyze the Carseats data set (library ISLR).
We use the ifelse() function to create a variable, called High, which takes on a value of Yes if the Sales variable exceeds 8, and takes on a value of No otherwise.
tree() function used to fit classification tree in order to predict High.
summary() function gives us the training error rate = 9%
plot() function used to display tree structure
The most important indicators of Sales seems to be shelving location.
In order to properly evaluate the performance of a classification tree on these data, we must estimate the test error rather than the training error. 
We split the observations in training set and a test set, build the tree using the training set, and evaluate its performance on the test data.
predict() function used for this purpose
The first predict() exercise using test and training set gives us a 71.5% prediction rate
Next, we prune the tree to see if it will yield better results.
The tree with 9 nodes results in lowest cross-validation error rate, with 50 cross-validation errors. 
The 9-node-tree is then constructed which gives us a 77% prediction rate. 
We plot then plot the 9-node-tree
