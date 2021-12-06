# Exploratory Data Analysis Collection

### Author : Gukhwan Hyun

## Introduction
This repository is my collection of Exploratory Data Analysis on subjects I find interesting or helpful.
I'd like to pursue my career in data science and I believe getting my hands dirty with real-life data is good way to kick it off :)
BTW, This is an ongoing and long-term project so if you don't see anything interesting at the moment, please come back later for new updates!

## Environments
Codes were written and run on Google Colab unless stated otherwise

## Topic 1 : Video Streaming Platforms
If you want to watch your favorite/popular moives or TV shows these days, your go to method would probably be to subscribe to some of OTT services.
But there are now too many streaming platforms to choose from and in so-called the age of streaming, it's quite common to face such a dilemma.
In addtion, they often use "Exclusive" contents to lure you in, making you feel exhausted already. So how would you decide which streaming platform is the best fit for you?

### Summary of Analysis
Categories are about the **most commonly appeared** on each platform.

| Category  | Netflix  | Disney+  | AmazonPrime  |
|---|---|---|---|
|Director|Rajiv Chilaka|Jack Hannah|Mark Knight|
|Cast|Anupam Kher|Jim Cummings|Maggie Binkley|
|Country|United States|United States|Not Available|
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
