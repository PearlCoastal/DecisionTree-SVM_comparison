# A simple experience of Desion Tree and SVM

A simple comparison experiment of supervised machine learning method: Decision Tree and SVM.

## Dataset

Dataset named "Penguin" imported from seaborn data.

url 👉 "https://raw.githubusercontent.com/mwaskom/seaborn-data/master/penguins.csv"

## Dataset pre-processing procedure

Because the initial dataset contains "species", "island" and "sex" which are string and I've transformed them into float using "replace"

Like in species there are three kinds : "Adelie, Chinstrap, Gentoo", and they are in "string"so I replace it with "0,1,2" which is in "float"

The island and sex are pre-processed as the same.

Here are the dataset after pre-processed.
![image](https://github.com/PearlCoastal/DecisionTree-SVM_comparison/blob/master/svm_dt/%E6%88%AA%E5%B1%8F0003-07-29%2017.37.41.png)

## Split the dataset into training set and test set

- using 'species', 'island', 'culmen_length_mm', 'culmen_depth_mm', 'flipper_length_mm', 'body_mass_g' as training feature
- using 'sex' as label

Seperate dataset into training and test set as train size as 8/10 and test size as 2/10.

![image](https://github.com/PearlCoastal/DecisionTree-SVM_comparison/blob/master/svm_dt/%E6%88%AA%E5%B1%8F0003-07-29%2017.46.17.png)

## Using Decision Tree and construct a tree first

Import tree from sklearn.

Because entropy is the expected value of information amount, so when entropy is high, its difficule to seperate, while entropy is low, its good.

So the criterion choose entropy in order to measure the quality or a split.

Then using plot function to train the tree.

Here is the Decision Tree.
![image](https://github.com/PearlCoastal/DecisionTree-SVM_comparison/blob/master/svm_dt/%E6%88%AA%E5%B1%8F0003-07-29%2017.52.25.png)

## Result of the Desicion Tree

![image](https://github.com/PearlCoastal/DecisionTree-SVM_comparison/blob/master/svm_dt/%E6%88%AA%E5%B1%8F0003-07-29%2017.38.08.png)

## Result of the SVM

![image](https://github.com/PearlCoastal/DecisionTree-SVM_comparison/blob/master/svm_dt/%E6%88%AA%E5%B1%8F0003-07-29%2017.38.26.png)

## Discussion of this comparison

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
