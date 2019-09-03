# Data-Analytics-Projects

Included in this repo are some interesting data manipulation and modelling projects that I worked on over the last few months. All analysis was performed in **python (Jupyter Notebook)**. Below is a brief introduction to each of the projects included. 

For more information on the individual projects including some interesting finds during exploratory analysis, please go into the sub-folders. Also looking to improve existing code and extend current functionality so if anyone has got interesting ideas or suggestions for future work, please do let me know!  


## Projects using Supervised Learning Models: 

1. Analysis on United Kingdoms road safety and traffic demographics dataset obtained from [UK Traffic Dataset - Kaggle](https://www.kaggle.com/tsiaras/uk-road-safety-accidents-and-vehicles#Accident_Information.csv) with the following key goals: 
    * Identify common factors responsible for higher accident rates through various feature engineering techniques
    * Carry out a restrospective study of the historical dataset and perform descriptive analysis (**Tableau, Power BI and Excel Power Pivot**)
    * Attempt to correct an imbalanced target class (**SMOTE, Cluster Centroid, Tomek Links**)
    * Perform hyper-paramter tuning using [GridsearchCV](https://scikit-learn.org/stable/modules/grid_search.html) (scikit-learn python package) to enhance predictive power of several supervised learning models (**KNN, SVM, Naive Bayes, Logistic Regression, Random Forest, Gradient Boost - Scikit-learn**)

2. Analyze several thousand tweets collected using [Twitters Streaming API](http://docs.tweepy.org/en/v3.5.0/api.html) in **JSON** format to perform sentiment analysis and classify them into sub categories for a more general consensus. The topic for this NLP project was the 106th **#Greycup/#greycup** held in Edmonton in November, 2018. Key analytic goals:
    * Perform a clean data pull from Twitter and transform data for analysis in python (**Tweepy**)
    * Various descriptive and time series analysis for insights (**matplotlib (Basemap), Mapboxgl**)
    * Build a predictive models to classify sentiment of a tweet (**textblob**)
 

   
 
    
