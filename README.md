# Exploratory Data Analysis Collection

### Author : Gukhwan Hyun

## Table of Contents
- [Exploratory Data Analysis Collection](#exploratory-data-analysis-collection)
  * [Introduction](#introduction)
  * [Environments](#environments)
  * [Topic 1 : Video Streaming Platforms](#topic-1--video-streaming-platforms)
    + [Summary of Analysis](#summary-of-analysis)
  * [Topic 2 : Customer Personality Analysis](#topic-2--customer-personality-analysis)
    + [Summary of Analysis](#summary-of-analysis-1)

## Introduction
This repository is my collection of Exploratory Data Analysis on subjects I find interesting or helpful.
I'd like to pursue my career in data science and I believe getting my hands dirty with real-life data is good way to kick it off :)
BTW, This is an ongoing and long-term project so if you don't see anything interesting at the moment, please come back later for new updates!

## Environments
Codes were written and run on Google Colab unless stated otherwise

## Topic 1 : Video Streaming Platforms
If you want to watch your favorite/popular moives or TV shows these days, your go to method would probably be to subscribe to some of OTT services.
But there are now too many streaming platforms to choose from also they often use "Exclusive" contents to lure you in, making you feel exhausted already. So now the question lies not in what but how. How can you decide which streaming platform is the best fit for you?

### Summary of Analysis
Categories are about the **most commonly appeared** on each platform.

| Category  | Netflix  | Disney+  | AmazonPrime  |
|---|---|---|---|
|Director|Rajiv Chilaka|Jack Hannah|Mark Knight|
|Cast|Anupam Kher|Jim Cummings|Maggie Binkley|
|Country of Production|United States|United States|Not Available|
|Genre|International Movies|Family|Drama|
|Rating|TV-MA|TV-G|13+|
|Duration(% of end in 1 season)|67%|55%|71%|

Quick Desicision Helper:
  * Looking for **adult** contents, **global** media contents --> **Netflix**
  * Looking for **family**, **kid** contents --> **Disney+**
  * Looking for extra contents such as meditation, Yoga, etc as well as regular movie and TV shows --> **AmazonPrime**

Also following questions were answered:
  * Persona (Relationship btw directors and actors)
  * Most common actors, genres per country
  * Most common directors, actors per genre
  * Most demanding directors, actors in past 5 years 


## Topic 2 : Customer Personality Analysis
Customer Personality Analysis is a detailed analysis of a company's ideal customers. In other words, it's a marketing strategy to tailor products or promotions to match the needs of the customers. Although the dateset does not specify where exactly data was collected, it appears to be from a relatively large grocery store.

### Summary of Analysis
Top Customers:

* NA : Outstanding group does not exist

|    |Age|Income|Child|Marital Status|Education|
|---|---|---|---|---|---|
|Wine|70s|Upper|0|Widow, Absurd|PhD |
|Meat|20s|6 figs|0|Absurd|NA|
|Fruit|NA|Upper|NA|Absurd|NA|
|Fish|20s, 70s|Upper|NA|Absurd|NA|
|Sweet|NA|6 figs|NA|Widow|NA|

1. Spending trend
   * Wine and meat are the most demanding products
   * Income, age are proportional to the spending
   * Spending on meat product is proportional to income
   * Number of kids and the spending are inversely proprotional 
   * Education level is proprotional to the spneding on wine
   * Amount of spending has decreased continuously from 2012 to 2014

2. Customer satisfaction
   * 0.95% complaint rate
   * Customer who complained took 5 more days to come back
   * Married customers in 40s and 60s with a college degree, middle income, one child filed the most complaint
   * Number of complaints doubled in 2013 and reduced by 75% in 2014.

3. Purchase pattern
   * Number of visit to website is proportional to number of purchase on web and purchase of the discounted products
   * Customers with the highest income tend to shop via a catalog
   * Tendency to shop via catalog increases as income increases
   * Customer with kids tend to shop on the discounted products
   * Absurd buys via catalog and YOLO buys via web and deal

4. Campaign (Promotional event) Results : top customer group
   * Campaign1 : 40s, 60s, Upper income, Married, zero kid or teen, graudation level
   * Campaign2 : 60s, 50s, Upper income, Togther, zero kid or teen, graudation level, PhD
   * Campaign3 : 40s, 50s, Middle income, Married, zero kid or teen, graudation level
   * Campaign4 : 50s, 60s, Upper, Middle income, Married, zero kid, 1 or 0 teen, graudation level
   * Campaign5 : 30s, 40s, 60s, 50s, Upper income, Married, zero kid or teen, graudation level


