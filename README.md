# sparkify_repo
Link for display of web page
https://r474340c796848xjupyterd00uxhei.udacity-student-workspaces.com/view/templates/sparkify_pr.html

Project Definition:
      Resilient Distributed Datasets is a fundamental Datastructure of Spark. It is an immutable distributed collection of objects. Each 
dataset in RDD is divided into logical partitions which may be computed on different nodes of the cluster.
      In this project we manipulate large and realistic datasets with Spark to engineer relevant features for predicting churn. We use 
Spark MLlib to build machine learning models with large datasets, far beyond what could be done with non-distributed technologies 
like scikit-learn.

Motivation:
      Keeping in view the large data being generated these days, I am interested to learn how to load large datasets into Spark and
manipulate them using Spark SQL and Spark Dataframes, use the machine learning APIs within Spark ML to build and tune models. In this 
project I integrated what I have learnt till now with Spark.This new skills I am learning gave me the driving force to complete the 
project.

Libraries used for this project are:
     Numpy, pandas, matplotlib.pyplot, pyspark_dist_explore, datatime, flask, from pyspark.sql import Window, from pyspark.sql.functions 
aggregate functions, from pyspark.ml.classification import NaiveBayes, RandomForestClassifier, from pyspark.ml.evaluation import 
MulticlassClassificationEvaluator, from pyspark.sql import SparkSession, from pyspark.ml.tuning import CrossValidator, ParamGridBuilder,
from pyspark.ml.feature import StandardScaler, VectorAssembler

Analysis:
     The project is divided into sections like:
     Load and Clean Dataset:  I have loaded and cleaned the dataset, checking for invalid or missing data - for example, records without 
userids or sessionids.
     Exploratory Data Analysis: I have performed EDA by loading a small subset of the data and doing basic manipulations within Spark. 
Created a column Churn. Performed some exploratory data analysis to observe the behavior for users who stayed vs users who churned. By 
exploring aggregates on these two groups of users, observing how much of a specific action they experienced per a certain time unit or
number of songs played.
     Feature Engineering:  I have written a script to extract the necessary features from the smaller subset of data and ensured that the 
script is scalable.
Modeling:
    Performed Split of the full dataset into train, test sets. For testing out several of the machine learning methods learned previously 
I used NaiveBayes and RandomForestClassifier. From my previous projects I have done in the classroom, RFC was giving good F1-Score when
hyperparameter tuning was performed correctly, So finally I have taken RFC to optimize the F1-Score metric and plotted the feature
importances.

List of Files:
    Sparkify.ipynb, In this file I have done Load and Clean Dataset, Load and Clean Dataset
    Sparkify-Copy1.ipynb, In this file I have done Load and Clean Dataset, and Modeling
    Sparkify-Copy2.ipynb, In this file I have loaded and used the flask library for the function I have written as a script.
    I have added the html versions of all the above files.
    I have added a templates folder.
    In the templates folder I have added the html code in 'sparkify_pr.html' which will display the visualizations in EDA and others.
    In the templates folder I have added another folder 'use_for_sparkify' which contains the visualizations in '.png' format
    I have added the screenshot of my output on web page.
    The link for display of the web page is:         
https://r474340c796848xjupyterd00uxhei.udacity-student-workspaces.com/view/templates/sparkify_pr.html
     
The Difficulties I faced:
       In the middle of coding for Feature Engineering I got an error  "java.lang.OutOfMemoryError no enough memory for aggregation"
 This was the first time I got this error and so I performed Google Search and finally decided that I will take another copy of notebook
 and do the remaining. I used 'persist function'. RDD persistance in spark is an optimization technique which I have written in the 
 notebook. 
 I wanted to tune best hyperparameters for RFC  trying out with variable number of trees etc.,but was afraid of the memory error.
 Learned to handle big data a bit. The data file is very large to load it here, so not doing it.
 
 Summary of the Results and Conclusion:
      All the outputs of the cells  in .ipynb files display the summary very clearly.
      The visualizations give good picture of results.
           
