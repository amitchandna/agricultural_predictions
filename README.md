# Capstone Project - General Assembly Data Science Immersive - Can we build a model that classifies countries for agricultural policy efficiently?
The purpose of this capstone project is to help increase the efficiency with which we can target agricultural policy across the world. Currently a large amount of global policy as it relates to agriculture revolves around utlising the framework of global north and global south to create these policies. While this policy is effective and useful for many fields, using it within the agricultural sector does not necessarily make sense as there are many edge cases that are present in this framework and thinking as it is applied in the present day and age. For this reason this project attempts to reframe this in a positive way that reclassifies countries based on things that matter for agricultural policies. These things are the use of fertilisers, the emissions of these fertilisers, the amount of food that is being produced by a country. These factors can then be used to predict whether a country is a net importer or exporter to determine how policy is outrolled. A net exporter country would be producing more food than it needs and is able to sustain life in other parts of the world while a net importer country would have trouble feeding itself (I know this is an INCREDIBLY simplified view of economics and does not take into account other goods that one country may have a comparative advantage in creating, but food is arguably the most important commodity on this planet). 

# Packages to install

The compulsory packages for this to work are Pandas, Seaborn, Pandas_Profiling(Not necessary but really nice to have), NumPy, sklearn(confusion_matrix, make_classification, RandomForestClassfier BaggingClassifier, GradientBoostingClassifier, AdaBoostClassifer, LogisticRegression, mean_squared_error, r2_score_accuracy_score, cross_val_score, train_test_split, GridSearchCV, KFold, KNeighborsClassifer, Pipeline, make_pipeline, StandardScaler, SVC, DecisionTreeClassifier) and last but not least pickle

# The Dataset

The data set has come from the Food and Agricultural Organisation of the United Nations. This dataset has been collected from 1967 to 2017 and has tracked the movement of fertilisers along with food products across the entire world. For each food product that has been imported, there is a line in this dataset that highlights how much of a food item like wheat has been traded across the world. This trade matrix is incredibly detailed and as a result provides a large amount of data that can be further refined for this model. As this data set was quite large, it was loaded into PostGreSQL on my local machine and the prelim data analysis was done this way. I have added an easier way to do this with pandas so that this data set can be downloaded and run through the code as is. 

# Pandas Profiling
This package was used to help inform the EDA process and help to ensure that a proper EDA was carried out as the data set was quite large before running pandas analyses on it. 

# Pipeline Creation
As the data needed to be scaled, and then further analysed, pipelines were created that could carry out this task and then a gridsearch was carried out to determine the best parameters for these models. Using these best parameters, the most effective model at predicting whether or not a country is an importer or exporter of agricultural goods based on multiple proxy indicators. 


