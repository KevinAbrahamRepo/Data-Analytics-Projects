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
![Picture1](https://user-images.githubusercontent.com/15803839/64131244-6469fe80-cd95-11e9-96da-4b3ea0a98278.png)

![Picture2](https://user-images.githubusercontent.com/15803839/64131246-6764ef00-cd95-11e9-96a6-d323171a5bcc.png)

![Picture3](https://user-images.githubusercontent.com/15803839/64131248-6a5fdf80-cd95-11e9-8194-0d01354566f9.png)

![Picture4](https://user-images.githubusercontent.com/15803839/64131249-6df36680-cd95-11e9-9d70-9815beead301.png)

![Picture5](https://user-images.githubusercontent.com/15803839/64131250-70ee5700-cd95-11e9-9c6f-912f40feefc7.png)

![Picture6](https://user-images.githubusercontent.com/15803839/64131254-75b30b00-cd95-11e9-9187-b3c02627dfcd.png)
