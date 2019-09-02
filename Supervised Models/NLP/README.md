# Natural Language Processing - #GreyCup:


Extract tweets for the **106th Grey Cup** Held in Edmonton on November 25, 2018 and perform sentiment analysis to classify tweets into one of positive, negative or neutral for this subject 

Use a two pronged approach to collect tweets:
* Gathered tweets from hashtag for Grey Cup - **#greycup**
* Gathered tweets with keywords - **Grey Cup, GreyCup**

All tweets were collected in **JSON** format and then converted to text in *Jupyter Notebook* for analysis 

*(My functions to collect tweets are based on [Alexander's Blog Post](https://galeascience.wordpress.com/2016/03/18/collecting-twitter-data-with-python/))*

To run the code, include the following libraries in your notebook file (pip install <library name>):

* import re
* from textblob import TextBlob
* import csv, pandas as pd, json, datetime as dt
* import os, sys, time

**Twitter Developers API (make sure to create a new developers account for TWITTER):**

1. access_token = "1058460791xxxxxxxxxxxxxxx"
2. access_token_secret = "1058460791xxxxxxxxxxxxxxx"
3. consumer_key = "1058460791xxxxxxxxxxxxxxx"
4. consumer_secret = "1058460791xxxxxxxxxxxxxxx"

*To use Basemap library for plotting points on a map, I followed [these instructions for Windows 10](https://stackoverflow.com/questions/18109859/how-to-install-matplotlib-basemap-module-on-windows-7-with-winpython-or-any-pyt/31713592#31713592)*

# GeoMap:
![Picture1](https://user-images.githubusercontent.com/15803839/63983541-26b75e00-ca95-11e9-888b-5edcb8eac43d.png)

# Tweets WordCloud:
![Picture2](https://user-images.githubusercontent.com/15803839/63983555-35057a00-ca95-11e9-870e-31070496988d.png)

# Gameday Peak:
![Picture3](https://user-images.githubusercontent.com/15803839/63983572-42baff80-ca95-11e9-8fc6-fb72068fe96c.png)
