# Exploratory Data Analysis Collections

### Author : Gukhwan Hyun

## Introduction
This repository is my collections of Exploratory Data Analysis on subjects I find interesting or helpful.
I'd like to pursue my career in data science and I believe getting my hands dirty with real-life data is good way to kick it off :)
BTW, This is an ongoing and long-term project so if you don't see anything interesting at the moment, please come back later for new updates!

## Environments
Codes were written and run on Google Colab unless stated otherwise

## Topic 1 : Netflix Movies and TV Shows 
Dateset contains listings of all the movies and TV shows available on Netflix along with the details such as cast, director, genre, duration, etc.

### Questions & Answers
**Q1.** 
What to do with the missing values in columns: director, cast, country, date_added, rating, duration. 

**A1.** 
"data_added" columns can not be guessed; therefore, remove rows w/ missing vales. For other columns, replace missing value w/ "Not Available"

**Q2.**
Are there any pattern in which how Netflix upload the videos?

**A2.**
Yearly : Majority of videos were uploaded in between 2018 and 2021
Monthly : Not much of pattern
Daily : A first day of the month seems to be the Netflix regular update period. (a lot of videos were uploaded)

**Q3.** 
Movies vs. TV shows

**A3.**
Definitely more movies availabe on Netflix (apprx. 7:3)

**Q4.** 
Any difference in countries?  
**A4.**
Movies are more common in US, India, UK, France presumably because they have either huge movie manufacturers like Hollywood and Bollywood.
On the other hand, TV shows are more common in South Korea, Japan, and Taiwan. 

**Q5.** 
Which director appeared the most often?

**A5.**
Rajiv Chilaka

**Q6.**
Which actor/actress appeared the most often in US and South Korea?

**A6.**
In US, Samuel L. Jackson(41), Fred Tatasciore(39), James Franco(36), Nicolas Cage(35)
In South Korea, 성동일(18) 김원해(15), 이경영(15), 남주혁(15), 박해준(15) 

**Q7.** 
what is the most common rating?

**A7.**
TV-MA, meaning that there are lots of contents made for adults on Netflix.

**Q8.** 
It seems like Netflix often finished the show with only one season.

**A8.**
True. About 67% of TV series ended with first season.

