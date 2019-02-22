# Project-1-Visualizing-time-series-data
CS 5331 - 001 

Video demo link: https://youtu.be/aWy7VEUYBQI  
Web link: https://hxdu.github.io/Project-1-Visualizing-time-series-data/  

## Introduction
  This project provides an interactive visualization of time series data: 2018 California wildfire tweets (Nov 08 – Nov 30) in 3 different aspects: 
  a. The total number of tweets collected & 2018 California wildfire tweets over time; 
  b. The top 10 topics generated by a LDA topic modeling model, each representing by 5 words; 
  c. The number of 2018 California wildfire tweets in the following categories: locations (in or out of California), rescue related or not.    
  
## Data set
2018 California wildfire tweets (from Nov 08 to Nov 30), searched from tweets collected during which time.   
Attributes collected: tweets ID, time, user name, tweets and locations. 
The csv file is simply a collection of preprocessing results. 

## Processing (in Python):
1. Search:
    Delete items with empty attribute(s).  
    Dynamically expand key words lists for searching by checking the qualified tweets and unqualified ones.
    Search key words list: wildfire; location in CA; location outside of CA; and rescue related.
2. Cleaning for topic modeling
    Remove non-ascii characters, urls, user name in retweets, hashtags, punctuation and stopwords.
    Get tokenized, lemmatized, build a dictionary for LDA topic modeling.
3. Train the model and get the top 10 topics generated by the model.    
![image](https://github.com/HXDU/Project-1-Visualizing-time-series-data/blob/master/topicsForVVA.png)

## Interesting findings:
   When talking about disaster tweets, we might wonder, what are people talking and what is the main topic wiring on different social medias. This project provides an instance view of such an answer.   
     First, despite of different categorizes, the number of wildfire tweets over time shows surprising consistence between one and each other.   
   Second, unsurprsingly, the number of wildfire related tweets hits the highest for the first few days and keeps decreasing after that. Although it is a state disaster that is commonly seen almost every year, 2018 California year caught national attentions due to its duration and the casualties it caused. Thus, the number of tweets marked within state of California stays close to those that are otherwise. 
   ![image](https://github.com/HXDU/Project-1-Visualizing-time-series-data/blob/master/Project1.png)
