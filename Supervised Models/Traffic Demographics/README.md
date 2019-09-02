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

### First point of impact: 
![Picture7](https://user-images.githubusercontent.com/15803839/64131308-b874e300-cd95-11e9-8d63-5ac83dcf86f7.png)

![Picture3](https://user-images.githubusercontent.com/15803839/64131248-6a5fdf80-cd95-11e9-8194-0d01354566f9.png)

![Picture4](https://user-images.githubusercontent.com/15803839/64131249-6df36680-cd95-11e9-9d70-9815beead301.png)

### Recursive Feature Elimination with CV - Logistic Regression:
![Picture5](https://user-images.githubusercontent.com/15803839/64131250-70ee5700-cd95-11e9-9c6f-912f40feefc7.png)

### All Model Performance Comparison:
![Picture6](https://user-images.githubusercontent.com/15803839/64131254-75b30b00-cd95-11e9-9187-b3c02627dfcd.png)

**Working with a highly imbalanced dataset with the majority class constituting 85% of all records, I used other metrics such F-Score, Recall, Mathews Correlation Coefficient MCC to determine the best model. Gaussian Naive Bayes performed marginally better for recall scores than Logistic Regression. The descision tree based models performed relatively poorly overall. The models can still be improved further through tuning parameters and possibly balancing target class.** 

*[Metrics to measure model performance for an imbalanced dataset](https://towardsdatascience.com/what-metrics-should-we-use-on-imbalanced-data-set-precision-recall-roc-e2e79252aeba)*

### Implications from Findings:
* Decrease emergency response times during *afternoon rush-hours (15-19) especially on Fridays*
* Allocate resources to investigate high density traffic points mapped above and identify new infrastructure needs to divert traffic from *dual-carriage ways*
* Explore conditions of vehicles and casualties such as vehicle type, age of vehicles registered, pedestrian movements, etc. for policy makers
* Adopt comprehensive distracted driving laws that increase penalties for drivers who commit traffic violations including aggressive overtaking which likely is also the reason for a majority of front end collisons. 


