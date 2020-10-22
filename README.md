# Data Science Immersive Capstone Project
## Can we build a model that classifies countries for agricultural policy efficiently?
  The purpose of this capstone project is to help increase the efficiency with which we can target agricultural policy across the world. Currently, a large amount of global policy, as it relates to agriculture, revolves around utilising the framework of global north and global south to create these policies. While this policy is effective and useful for many fields of study, using it within the agricultural sector does not make sense as there are far too many special cases in the agricultural sector. 

  For the reasons listed above, this project attempts to reframe this in a positive way that reclassifies countries based on things that matter for agricultural policies. These things are the use of fertilisers, the emissions of these fertilisers, and the amount of food that is being produced by a country. These factors can then be used to predict whether a country is a net importer or exporter to determine how policy is outrolled. A net exporter country would be producing more food than it needs and is able to sustain life in other parts of the world while a net importer country would have trouble feeding itself.

  The goal of this project was to create a model that can determine whether or not the strength of a countries agricultural sector could be predicted based on proxy indicators. These proxy indicators can then demonstrate whether or not our classification of a country as a developed or developing country has any real weight when it comes to how policy is outrolled. This project has demonstrated that a countries agricultural success is not related to whether or not it is a developed or developing country and can be predicted based on other indicators such as greenhouse gas emmissions from the agricultural sector.
  
##[The Data Set](http://www.fao.org/faostat/en/#home) - Navigate to the bulk data download

## Packages to install
The compulsory packages for this to work are as follows:
* Pandas
* Seaborn 
* Pandas_Profiling(Not necessary but really nice to have)
* NumPy
* Pickle
* sklearn with each of the following packages
  - confusion_matrix
  - make_classification
  - RandomForestClassfier 
  - BaggingClassifier
  - GradientBoostingClassifier
  - AdaBoostClassifer
  - LogisticRegression
  - mean_squared_error
  - r2_score_accuracy_score
  - cross_val_score
  - train_test_split
  - GridSearchCV
  - KFold
  - KNeighborsClassifer
  - Pipeline
  - make_pipeline
  - StandardScaler
  - SVC
  - DecisionTreeClassifier


## The Dataset

The dataset has come from the Food and Agricultural Organisation of the United Nations. This dataset has been collected from 1967 to 2017 and has tracked the movement of fertilisers along with food products across the entire world. For each food product that has been imported, there is a line in this dataset that highlights how much of a food item like wheat has been traded across the world. This trade matrix is incredibly detailed, and as a result, it provides a large amount of data that can be further refined for this model. As this dataset was quite large, it was loaded into PostGreSQL on my local machine and the preliminary data analysis was done this way. I have added an easier way to do this with Pandas so that this dataset can be downloaded and run through the code as is. 

## Pandas Profiling
This package was used to help inform the EDA process and help to ensure that a proper EDA was carried out as the dataset was quite large before running Pandas analyses on it. 

## Pipeline Creation
As the data needed to be scaled, and then further analysed, pipelines were created that could carry out this task and then a gridsearch was carried out to determine the best parameters for these models. Using these best parameters, the most effective model at predicting whether or not a country is an importer or exporter of agricultural goods based on multiple proxy indicators was created to model this scenario. 

## Results

Essentially what has been created here is a model that reclassifies countries based on whether or not they are importing or exporting food using proxy indicators and does so quite accurately. The model that has been created classifies a country with 94% accuracy. This model can be subsequently used to work towards creating a better idea of which countries should be held accountable for imports and exports, as it relates to agricultural products as net importers should likely pay a higher carbon tax than those that are net exporters, as the net importing countries are more reliant on the global system to feed themselves. This is the cornerstone of any countries' success and should be treated as such. 

## Perspectives
This project was completed as my first full length data science project from a question being asked, to the collection of the dataset, to the creation of a model to answer my question. It had many ups and downs as the first project will, but ultimately each of the problems that arose were easily solved through some grit and referencing stack overflow. To make this project even better, I would further create a neural network and superimpose it upon a world map in Tableau. This would help to demonstrate the direction of various food products and visually show which countries are providing for themselves and which countries are relying on other countries to support them. All these things considered, this was a very successful first data science project that has demonstrated both my skills in data analytics along with a potential new way to frame the world around us.  
