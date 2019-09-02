# Natural Language Processing - #GreyCup:


For this mini-project I extracted tweets for the **106th Grey Cup** Held in Edmonton on November 25, 2018 and performed sentiment analysis to classify tweets into one of positive, negative or neutral 

### Use a two pronged approach to collect tweets:
* Gathered tweets from hashtag for Grey Cup - **#greycup**
* Gathered tweets with keywords - **Grey Cup, GreyCup**

*(My functions to collect tweets are based on [Alexander's Blog Post](https://galeascience.wordpress.com/2016/03/18/collecting-twitter-data-with-python/))*


**You will require a developers account for TWITTER to retrieve keys/tokens:**

1. access_token = "1058460791xxxxxxxxxxxxxxx"
2. access_token_secret = "1058460791xxxxxxxxxxxxxxx"
3. consumer_key = "1058460791xxxxxxxxxxxxxxx"
4. consumer_secret = "1058460791xxxxxxxxxxxxxxx"

### Mapbox Python SDK:
![Picture1](https://user-images.githubusercontent.com/15803839/63983541-26b75e00-ca95-11e9-888b-5edcb8eac43d.png)
**Top 3 Locations:**
1. Calgary, Alberta
2. Edmonton, Alberta
3. Toronto, Ontario

*Alternatively you can use Basemap library for plotting points as well, I followed [these instructions for Windows 10](https://stackoverflow.com/questions/18109859/how-to-install-matplotlib-basemap-module-on-windows-7-with-winpython-or-any-pyt/31713592#31713592)*

### Tweets WordCloud:
![Picture2](https://user-images.githubusercontent.com/15803839/63983555-35057a00-ca95-11e9-870e-31070496988d.png)
**Top Tweeted Words:**
1. greycup 
2. Grey
3. Cup 
4. cfl (Canadian football league)

### Gameday Tweets Frequency:
![Picture3](https://user-images.githubusercontent.com/15803839/63983572-42baff80-ca95-11e9-8fc6-fb72068fe96c.png) 

**Most twitter activity was recorded on November 24 & 25, 2018**

### Tweet Sentiments using TextBlob: 
![Picture4](https://user-images.githubusercontent.com/15803839/64128118-e1d84380-cd82-11e9-96f6-5ce7967f1a7c.png)

