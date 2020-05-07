# CoronavirusTweet
Author: Sukyoung Cho & Hannah Wang  
  
The app serves to allow users to explore the tweets under #coronavirus, and plot the relationships between COVID-19 cases and tweet posts. To be more specific, it's the linear relationship that will be displayed.
  
Here's the app: https://hannahwang.shinyapps.io/CoronavirusTweet/

*Please refer to the "Usage" session for a smoother user experience. Due to the larger data size, please wait a second for figures to load. Or, please refresh the page when things are not showing up.*

## Introduction
Coronavirus disease (COVID-19) is an infectious disease with unprecedentedly extreme contagiousness, which is far beyond SARS or MERS. Its first outbreak was observed at Wuhan, the capital of Hubei province in China, and it is a catastrophe on a global scale. While it is spreading all over the world, the speed or the pattern of how it is transmitted varies by country. There could be factors such as the governments’ reactions that interfere with the spreading speed, but we want to delve into the social media perspective to investigate if it can predict the spread of COVID-19.
 
The initial thought is that social media is a platform where people discuss things they care about. Regarding COVID-19, there are so many online discussions every day. Thus, we are curious to examine if these discussions have anything to do with the spread of disease. In this application, tweets under the #coronavirus hashtag are used as the proxy for COVID-19 related social media discussions. As for indices of the disease spread, total confirm cases, total test cases, confirm cases per 100 tests, new cases, new deaths, and total deaths are included to let users explore. With the tweets data collected from Twitter API, and coronavirus data from Our World in Data website, we found two ways to account for the variations in the COVID-19 case numbers: one is the topic clusters of the tweets which is shown in the "Tweet Wall" tab, and the other is the frequent words within tweets.

## Methods
### Data Sources & Data descriptions
1. Tweet data source: tweets were collected from Twitter API, and the twitter accounts were further divieds into flocks, the work was done by Karl's lab, which is same as the [murmuration website](https://murmuration.wisc.edu/historical/2020-05-04#event-1). 

<needs to put a screen shot of the twitter data and describe each columns>
 
2. Covid-19 case data source: our complete COVID-19 dataset is a collection of the COVID-19 data maintained by [Our World in Data](https://ourworldindata.org/coronavirus). The repo for raw data can be found [here](https://github.com/owid/covid-19-data/tree/master/public/data). It is updated daily and includes data on confirmed cases, deaths, and testing. The data are updated up-to-date. We used the data of the United States only and the data ranging only from Feb 1st to March 31st to match with the twitter data. The data are mainly from the ECDC (European Centre for Disease Prevention and Control) and the WHO (World Health Organization).

<needs to put a screen shot of the covid-19 data and describe each column>

### Data Cleaning
All codes for data cleaning are included in the dataprocessing.Rmd file. 

### Statistical Techniques
1. Tweet Explore

2. Tweet Wall

3. Spread of Covid-19 v.s. frequent words

## Usage of the App
<include gif for each tab>
  
1. Tweet Explore

2. Tweet Wall

3. Spread of Covid-19 v.s. frequent words

## Results
<give an example for each tab>
  
1. Tweet Explore

2. Tweet Wall

3. Spread of Covid-19 v.s. frequent words

## Conclusions
<Summarize evidence and limitations>

Using the ShinyR package, the app successfully displayed the twitter data and the Covid-19 data with plenty of graphics and interactivity. In our app, users are allowed to navigate the data in their own ways, which dramatically escalated the readability of the data even to users who do not have statistical knowledge. There are some ways this app could be improved. For example, the predictors for the linear model could be changed with user’s interest. For example, a user might want to see the relationship between Covid-19 data and the most frequent words on the specific day and in a specific flock of interest.
