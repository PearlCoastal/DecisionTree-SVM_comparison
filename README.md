# A simple experience of Desion Tree and SVM

A simple comparison experiment of Decision Tree and SVM.

## Dataset

## Discussion

Discison Tree is easily to interpret, and easily to be trained.

And because there are several missing values in 'penguin' dataset, and Decision Tree is good dealing with dataset with missing values.

SVM are supervised models with associated learning algorithm that analyze data used for classification and regression analysis, based on the statistical learning framework.

An SVM model performe better when dealing with high-dimentional space dataset, but when dealing with datasets which are at same space and predicted to belong to a category based on the side of the gap on which they fall.

So as in my experiment when 'penguin' datasets are using an SVM model, the accuracy and F1-score are way lower than its in Decision Tree.

## Data Analysis

As you can see the results above.

The Accuracy of Decision Tree is 0.9253731343283582

while the Accuracy of SVM is 0.6716417910447762

So Decision Tree is better than SVM in Accuracy.

And as the F1 score is a measure of a test's accuracy. It considers both the precision and the recall of the test to compute the score.

The F1 score of Decision Tree = 0.9315068493150686

and the F1 score of SVM = 0.7027027027027027

So under the dataset of penguin, Decison Tree performed better than SVM.

## Result

In conclusion, in my consideration, Decision tree performs better when dealing with datatsets with missing values while SVM is not.

And SVM performs better when dealing with high-dimentional space but 'penguin' is not, so the results of accuracy and F1-score are not as good as its in Decision Tree.
