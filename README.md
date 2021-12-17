# Exploratory Data Analysis Collection

### Author : Gukhwan Hyun

## Table of Contents
- [Exploratory Data Analysis Collection](#exploratory-data-analysis-collection)
  * [Introduction](#introduction)
  * [Environments](#environments)
  * [Topic 1 : Video Streaming Platforms](#topic-1--video-streaming-platforms)
  * [Topic 2 : Sales](#topic-2--Sales)

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


## Topic 2 : Sales

### Objective
탐색적 데이터 분석 (Exploratory Data Analysis, EDA) 를 통해 데이터 속 변수들 간의 상관관계와 그로부터 추론된 인사이트(Insight) 를 이용하여 판매 전략을 도출한다.


### Dataset

1. Customer Personality Analysis (CPA) :
 
	CPA 는 기업의 고객층을 분석해서 목표 고객에 최적화된 상품이나 전략을 짜도록 돕는 고객 분석 전략이다.

	**원본데이터** (2,240 rows by 29 cols) :
	
	나이, 교육수준, 결혼여부, 수입, 자녀, 품목별 소비량 (와인, 과일, 육류, 수산물, 당류), 구매처 (웹, 카탈로그, 가게), 할인행사 참여도 등 고객 상태에 따른 소비성향을 알 수 있는 데이터로 구성되어 있음.

	**분석데이터** (2,216 rows by 35 cols) :
	
	연령별 그룹(10~70대), 소득수준별 그룹(최상, 상, 중, 하), 구매기간 (연, 월, 일) 등 통계적 분석이 가능하도록 데이터를 가공하여 추가하였음. 


2. Sales Product Data (SPD) :

	SPD 는 판매 제품, 트렌드, 판매처 등을 분석해서 미래 판매 전망을 예측하고, 현재 상태를 분석하는 제품 분석 전략이다.

	**원본데이터** (186,850 rows by 6 cols) :
	
	주문번호, 상품, 수량, 가격, 주문시간, 배송주소 등 Amazon 에서 물품을 구매하면 생성되는 데이터로 구성되어 있음. 

	**분석데이터** (185,950 rows by 13 cols) :
	
	주문 총 판매금액, 주문시간 (연, 월, 일, 시), 배송주소 (도시, 주) 등 통계적 분석이 가능하도록 데이터를 가공하여 추가하였음.


### Data Analysis

1. Customer Personality Analysis (CPA) :

	**소비성향** :

	* 육류와 와인은 가장 많이 팔리는 품목이다.
	* 소득수준과 나이는 소비와 양의 상관관계를 가진다.
	* 자녀의 숫자와 소비는 음의 상관관계를 가진다.
	* 교육수준과 와인소비량은 양의 상관관계를 가진다.
	* 전체 소비량은 지속적인 감소 추세에 있다.

	**고객만족도** :

	* 전체 고객 중 약 0.95% 의 고객이 불만족을 표시했다. 
	* 불만족을 표시했던 고객은 재방문까지 평균 5일 이상의 시간이 더 걸렸다.
	* 주로 불만족을 표시한 고객은 대학교 학위를 가지고 중산층에 속하며, 자녀가 있는 40대, 60대였다.
	* 2013년에는 고객불만족이 2배 증가했다가, 2014년에는 75% 감소하였다.

	**구매패턴** :

	* 웹사이트 방문률과 온라인 구매 및 할인 상품 구매량은 양의 상관관계를 가진다.
	* 최상위 소득수준의 고객은 주로 카탈로그를 통해 구매를 하였다. 그리고 소득 수준이 증가할 수록 카탈로그로 구매하는 경향이 더 많아졌다. 
	* 자녀가 있는 고객은 할인 상품을 구매하는 경향이 많았다.

	**판촉행사별 주 참여 고객** :

	* 1번행사 : 상류층에 속한 자녀가 없는 40대, 60대 
	* 2번행사 : 박사학위가 있고, 상류층에 속한 자녀가 없는 50, 60대 
	* 3번행사 : 중산층에 속한 자녀가 없는 40, 50대
	* 4번행사 : 중산층, 상류층에 속하며, 1명이상의 자녀가 있는 50, 60대
	* 5번행사 : 상류층에 속한 자녀가 없는 30~50대 

2. Sales Product Data (SPD)

	**판매** :

	2019년도 1월이 가장 적고, 12월이 가장 높은 판매금액을 보였다.

	1월-4월은 판매금액이 상승, 4월-9월은 판매금액이 하락, 9월-12월은 판매금액이 다시 상승하였다.  

	샌프란시스코가 가장 높은 판매 금액을 보였다. 그외에도 대체로 서부지역이 동부지역보다 높은 판매금액을 보였다.

	12시, 19시에 판매량은 최고점을 보였다.

	4-12시까지 판매량은 상승곡선을 보이고, 12시-15시까지 하강곡선을 보이다가 15-19시까지 다시 상승하는 경향을 보였다.

	따라서 물품 판매량을 올리기 위한 광고는 9시, 15시를 기점으로 하는 것이 좋아보인다.

	스마트폰과 충전케이블은 같이 판매되는 경향이 많았고, 충전케이블과 배터리는 최상위 판매량을 보였다. 




