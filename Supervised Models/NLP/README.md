# Natural Language Processing (Text Analytics) - #GreyCup:


For this project I extracted tweets for the **106th Grey Cup** Held in Edmonton on November 25, 2018 and performed sentiment analysis to classify tweets into one of positive, negative or neutral 

## Python Packages Used: 
* Scikit-Learn, Numpy, Pandas, Mapboxgl, NLTK, Matplotlib, Tweepy

## Used a Two Pronged Approach to Collect Tweets:
* Gathered tweets from hashtag for Grey Cup - **#greycup**
* Gathered tweets with keywords - **Grey Cup, GreyCup**

*My functions to collect tweets are based on [Alexander's Blog Post](https://galeascience.wordpress.com/2016/03/18/collecting-twitter-data-with-python/)*

*Heres another interesting read [on an introduction to using Twitters streaming API](http://adilmoujahid.com/posts/2014/07/twitter-analytics/)*


**NOTE: You will require a developers account for TWITTER to stream and extract tweets live**

1. access_token = "xxxxxxxxx"
2. access_token_secret = "xxxxxxxxx"
3. consumer_key = "xxxxxxxxx"
4. consumer_secret = "xxxxxxxxxx"

*I referred to [this blog](https://medium.com/@jayeshsrivastava470/how-to-extract-tweets-from-twitter-in-python-47dd07f4e8e7) on instructions to get TWITTER API keys*

## Data Cleansing Steps:
Please review **Data_Cleansing_Functions** python file for common functions used to prepare data for analysis + modelling 

## Exploratory Analysis (EDA):

## Mapbox Python SDK:
![Picture1](https://user-images.githubusercontent.com/15803839/63983541-26b75e00-ca95-11e9-888b-5edcb8eac43d.png)
**Top 3 Locations:**
1. Calgary, Alberta
2. Edmonton, Alberta
3. Toronto, Ontario

*Alternatively you can use **Basemap** library for plotting points as well. Follow [these instructions for Windows 10](https://stackoverflow.com/questions/18109859/how-to-install-matplotlib-basemap-module-on-windows-7-with-winpython-or-any-pyt/31713592#31713592)*

## Common Words in Tweets - WordCloud:
![Picture2](https://user-images.githubusercontent.com/15803839/63983555-35057a00-ca95-11e9-870e-31070496988d.png)
**Top Tweeted Words:**
1. greycup 
2. Grey
3. Cup 
4. cfl (Canadian football league)

## Gameday Tweets Frequency - R Studio:
![Picture3](https://user-images.githubusercontent.com/15803839/63983572-42baff80-ca95-11e9-8fc6-fb72068fe96c.png) 

*Most twitter activity was recorded on **November 24 & 25, 2018** as expected.*

## Tweet Sentiments - TextBlob Python Library: 
![Picture4](https://user-images.githubusercontent.com/15803839/64128118-e1d84380-cd82-11e9-96f6-5ce7967f1a7c.png)


## Code + Models Tested:

There are two versions of the code I worked on simultanously that I hope to eventually combine into one. 

* **Part 1** includes a more detailed approach to extracting and analysing the tweets. This also includes a few supervised models that were run to predict the sentiment of a tweet:
  * Naive Bayes - 87% accuracy
  * Support Vector Machine (Linear Kernel) - 95% accuracy
  * Support Vector Machine (Polynomial Kernel) - 20% accuracy (will need to tune parameters further)
  
* **Part 2** includes some general exploratory analysis. 

**NOTE: All libaries used have been listed in each of the python code files in detail. Have a go at it!**  


