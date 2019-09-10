## ANALYSIS OF ROAD SAFETY AND TRAFFIC DEMOGRAPHICS IN THE UK

For this project, the goal was to help provide recommendations to UK’s department of Transport - to improve road safety policies and prevent accident recurrences where possible. Implemented suggestions could be tested against the predictive model designed to identify the severity of an accident. 

The original dataset was retreived from [Kaggle - UK Traffic Dataset](https://www.kaggle.com/tsiaras/uk-road-safety-accidents-and-vehicles#Accident_Information.csv) 

### PYTHON PACKAGES USED:
* Scikit-learn, Numpy, Pandas, imblearn (imbalanced-learn), Seaborn, Matplotlib

### PRIMARY ANALYTIC GOALS: 
1. Identify common factors responsible for higher accident rates through various feature engineering techniques
   * PCA, RFECV, Variance Threshold, RandomForest Feature Importance
2. Carry out a restrospective study of the historical dataset and perform descriptive analytics using Tableau, Power BI and Excel Power Pivot to gain insights
3. Attempt to correct an Imbalanced target class using SMOTE, Cluster Centroid, Tomek Links (**imblearn** python library)
   * Referred to [resampling strategies post](https://www.kaggle.com/rafjaa/resampling-strategies-for-imbalanced-datasets) to implement various strategies to work with an imbalanced target class
4. Perform hyper-paramter tuning using *GridsearchCV* (**scikit-learn python** package) to optimize predictive power of several supervised learning models *(KNN, SVM, Naive Bayes, Logistic Regression, Random Forest, Gradient Boost)*


### DATA CLEANSING STEPS:
Please review **'Data_Cleansing_Steps'** python file on steps taken to prepare the data for descriptive analysis & modelling 


### EXPLORATORY DATA ANALYSIS 
EDA was completed in Tableau/MS PowerBI**

### Yearly Accident Rates:
![11](https://user-images.githubusercontent.com/15803839/64583797-5b15fe80-d360-11e9-926d-b85e95766c47.png)

### Age Group & Day-Time of Reported Accidents:
![Picture1](https://user-images.githubusercontent.com/15803839/64131244-6469fe80-cd95-11e9-96da-4b3ea0a98278.png)
![Picture2](https://user-images.githubusercontent.com/15803839/64131246-6764ef00-cd95-11e9-96a6-d323171a5bcc.png)

### First Point of Impact: 
![Picture7](https://user-images.githubusercontent.com/15803839/64131308-b874e300-cd95-11e9-8d63-5ac83dcf86f7.png)

*Its interesting to note that the majority of accidents reported were those of vehicles involved in a front end collision. This could potentially be a result of either **distracted driving, poor spatial judgement or impatient drivers.***

### Road Traffic Accident Density by Location:
![Picture3](https://user-images.githubusercontent.com/15803839/64131248-6a5fdf80-cd95-11e9-8194-0d01354566f9.png)

***Top Locations:** Birmingham, London, Leeds, Newcastle*

### Weather Conditions:
![Picture4](https://user-images.githubusercontent.com/15803839/64131249-6df36680-cd95-11e9-9d70-9815beead301.png)

*I would imagine that as weather conditions get worse, accidents reported would likely increase. However, the data suggests that most accidents occured when the conditions were perfectly normal especially during peak rush hours as observed earlier obove. Now it can also be argued that fewer cars may have been on the roads when driving conditions were poor. Unfortunately the dataset does not provide a count of vehicles on the road for those periods.*

### Road Types with Most Accidents Reported (Tree map): 
![Picture8](https://user-images.githubusercontent.com/15803839/64207763-466ecd80-ce6b-11e9-908c-c52b625919aa.png)


### Optiomal Features Suggestion through RFECV - Logistic Regression:
![Picture5](https://user-images.githubusercontent.com/15803839/64131250-70ee5700-cd95-11e9-9c6f-912f40feefc7.png)
*About 30 features accounted for roughly 95%+ of all variations* 

### Top Features Identified (RFECV-Logistic Regression):
1. Number of Vehicles Involved/ Casualties
2. Engine Capacity CC
3. Speed Limit
4. Age band of driver
5. Day of the week – FRIDAY
6. Daytime afternoon rush (15-19)
7. Light Conditions – DARK/NIGHT
8. Location (Latitude/Longitude)
9. Weather Conditions – Fine with NO High Winds
10. Age of the Vehicle 


### Model Comparison:
![Picture6](https://user-images.githubusercontent.com/15803839/64131254-75b30b00-cd95-11e9-9187-b3c02627dfcd.png)

### Target Class Imbalance: 
![Imblanace](https://user-images.githubusercontent.com/15803839/64583295-7bdd5480-d35e-11e9-9d1f-7946e9eaef83.png)

**Since the majority class constituted for roughly 85% of all records, other metrics such F-Score, Recall, Mathews Correlation Coefficient MCC were used to determine the best model. *Gaussian Naive Bayes* performed marginally better for recall scores than Logistic Regression to show the ratio of correctly predicted positive observations. The descision tree based models (Random Forest, Gradient Boost) performed relatively poorly overall.**

**NOTE: The results are lower than typical classification results, but this is primarily because of a highly imbalanced target class that expectedly introduces bias for the majority class while modelling. Each models can still be improved by balancing target class further and tuning model parameters.** 

*I referred to this article for [**metrics to measure model performance for an imbalanced dataset.**](https://towardsdatascience.com/what-metrics-should-we-use-on-imbalanced-data-set-precision-recall-roc-e2e79252aeba)*

### IMPLICATIONS FROM FINDINGS:
* Decrease emergency response times during **afternoon rush-hours (15-19) especially on Fridays**
* Allocate resources to investigate **high density traffic points** mapped above and identify new infrastructure needs to divert traffic from **dual-carriage ways**
* Explore conditions of vehicles and casualties such as **vehicle type, age of vehicles registered, pedestrian movements**, etc. for policy makers
* Adopt comprehensive distracted driving laws that increase penalties for drivers who commit traffic violations including aggressive **overtaking**


