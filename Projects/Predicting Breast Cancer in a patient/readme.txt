Title: Predicting Breast Cancer in a patient

Problem Statement:

Given the details of cell nuclei taken from breast mass, predict whether or not a patient has breast cancer using the Ensembling Techniques. Perform necessary exploratory data analysis before building the model and evaluate the model based on performance metrics other than model accuracy.

Steps involved:

Findings from the dataset:

1. The dataset is comprising of 569 instances with a total of 31 features along with a target ( diagnosis ) which is either B or M. B stands for Benign' meaning that the cells are not harmful or there is no cancer and M stands for 'Malignant' meaning that the patient has cancer and the cells have a harmful effect.

2. Out of 569 instances the targets bearing ‘B ‘are 357 and ‘M’ are 212. Hence, dataset is not imbalanced. All the features are of float datatype. 

3. With the histplot of the dataset it is evident that only a few of the features are normally distributed while, most of them are right skewed. Hence, calling for feature scaling.

Performed Exploratory Data Analysis to ,

1. Find the relationship between the important features as a pair to explore their impact on target

2. Find the relationship between the important features and target

Plotted heatmap with the help of df.corr() function to display the realtionship among the features , feature and target. 

Findings : 
1. 4 features are negatively correlated with the target, while the rest are positively correlated
2. Features with the negative correlation doesn’t have much of an impact on the target
3. Nearly 10 features show a strong positive correlation with the final outcome

> Set the benchmark by recording metrics like accuracy,prescision,recall,F1 score for the original dataset before performing scaling and hyper parameter tuning 

> Performed Standard scaling and recorded metrics like accuracy,prescision,recall,F1 score

> Performed GridSearch to find the best hyper parameters for SVM and Ensemble models [ RANDOM FOREST, BAGGING, ADA-BOOST, GRADIENT-BOOST, EXTREME-GRADIENT-BOOST CLASSIFIERS ]

> Built the above mentioned models with the hyper-parameters and recorded metrics like accuracy,prescision,recall,F1 score

> Compared the recorded metrics for original dataset, scaled dataset and hyper parameter tuned datasets

> Plotted sun-burst chart to visually explore the metrics of all the models

> with the help of data established supremacy of SVC over ensemble models






