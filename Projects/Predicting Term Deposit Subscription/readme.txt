Title : Predicting Term Deposit Subscription by a client

Problem statement : 

Predict if a customer subscribes to a term deposits or not, when contacted by a marketing agent, by understanding the different features and performing predictive analytics

Findings from the dataset:

1. No Null Values

2. The mean value of features is on different scale for most of the features.Hence, Scaling is required

3. The target has 36458-No and only 4640-Yes. Hence, the dataset is imbalanced

4. With the boxplot it is evident that there are outliers need to perform standard scaling

5. Histplot shows only few features are normally distributed, while the rest are skewed

Performed Exploratory Data Analysis to,

1. Find the relationship between the important features as a pair to explore their impact on target

2. Find the relationship between the important features and target

Plotted heatmap with the help of df.corr() function to display the realtionship among the features , feature and target. 

Findings : 
1. 8 features are negatively correlated with the target, while the rest are positively correlated

2. 10 features show  positive correlation with the final outcome

Set the benchmark by recording metrics like accuracy,precision,recall,F1 score for the original dataset with (80:20, 75:25, 70:30 train-test split ) before performing scaling and hyper parameter tuning 

> In order to balance the imbalanced dataset tried - Under sampling, Over sampling and SMOTE ( Synthetic Minority Over-sampling TEchnique ) , found out SMOTE out-performed the other 2 methods

> Performed Standard scaling and recorded metrics like accuracy,precision,recall,F1 score

> Performed GridSearch to find the best hyper parameters for SVM and other ML models [ LOGISTIC REGRESSION, KNN, RANDOM FOREST, BAGGING, ADA-BOOST, GRADIENT-BOOST, EXTREME-GRADIENT-BOOST CLASSIFIERS ]

> Built the above mentioned models with the hyper-parameters and recorded metrics like accuracy,prescision,recall,F1 score

> Compared the recorded metrics for original dataset, scaled dataset and hyper parameter tuned datasets

> Plotted sun-burst chart to visually explore the metrics of all the models

> Found out the Bagging classifier does the best job for the given dataset with SMOTE sampling, Standard scaling and hyper-parameter tuning with a F1-Score of 0.94 and an accuracy of 95%

> Among the various instanced of SVC, SMOTE scaled dataset with default hyper parameters performed the best


