# Analysis of Road Safety and Traffic Demograhics in UK

For this project, the goal was to help provide recommendations to UK’s department of Transport - to improve road safety policies and prevent accident recurrences where possible. Any implemented suggestions could be tested against the predictive model designed to identify the severity of an accident. 

The original dataset was retreived from [Kaggle - UK Traffic Dataset](https://www.kaggle.com/tsiaras/uk-road-safety-accidents-and-vehicles#Accident_Information.csv) 

Primary Analytic Goals: 
1. Identify common factors responsible for higher accident rates through various feature engineering techniques
2. Carry out a restrospective study of the historical dataset and perform descriptive analytics using Tableau, Power BI and Excel Power Pivot
3. Attempt to correct an Imbalanced target class using SMOTE, Cluster Centroid, Tomek Links (**imblearn** python library)
4. Perform hyper-paramter tuning using *GridsearchCV* (**scikit-learn python** package) to enhance predictive power of several supervised learning models *(KNN, SVM, Naive Bayes, Logistic Regression, Random Forest, Gradient Boost)*

*I referred to [resampling strategies post](https://www.kaggle.com/rafjaa/resampling-strategies-for-imbalanced-datasets) to implement various strategies to work with an imbalanced target class*

## Exploratory Data Analysis performed in Tableau/MS PowerBI:
