# ![Crumbl Cookie Logo](Crumbl.png) 

# Project 1: World Development Statistics


### Problem Statement

Crumbl Cookies is a family owned cookie company that was started by cousins Jason McGowan (CEO) and Sawyer Hemsley (COO). It was started in Logan, Utah, USA in 2017. In the seven years since its inception it has had tremendous success franchising in the US. They recently opened their 1000th location. They have grown so quickly, they've been dubbed the fasted growing dessert company in the United States.

They are looking to the future and their goal is to grow internationally. As one of their data scientists, they would like recommendations for viable markets outside the United States with an emphasis on populations that would support growth and expansion, robust economies, daily incomes and, most importantly, sugar intake. They are a cookie company after all. With international growth in mind, we are looking to answer the question of which country will offer the opportunity for continued growth.

---

### Datasets

Data Dictionary:

|Feature|Type|Dataset|Description|
|---|---|---|---|
|**gdp**|*float*|Year 2024| Predicted Gross Domestic Product per person adjusted for differences in purchase power in international dollars
|**population**|*float*|Year 2024|The population of Australia, Brazil, Canada, Denmark, Ireland, Japan, Mexico, Netherlands, New Zealand, Norway, Singapore, Switzerland, United Kingdom, United Stats (Predicted population expected).|
|**income**|*float*|Year 2024|The average daily income per capital|
|**sugar**|*float*|Year 2018|The most recent data on quantity of consumption of sugar and sweeteners in grams per person per day.|

#### Project Datasets

There are 4 datasets included in this project. They are the GDP, Population, Daily income and Sugar per person. All four datasets came from Gapminder at (https://www.gapminder.org/data/).


#### Additional Data
In my slide presentation I reference that Crumbl Cookies is the fastest growing dessert company in the United States. That reference is per the New York Times post found here (https://www.nytimes.com/2023/04/17/dining/crumbl-cookies.html#:~:text=Crumbl%20is%20the%20fastest%2Dgrowing,stores%20from%20coast%20to%20coast.)

---

### Executive Summary
My process in approaching this project was to find data relevant to a global expansion. Crumbl Cookies is a family owned business in the US. In this hypothetical project they need suggestions as to which countries offer the best likelihood for success. I chose to limit the scope of the project to 14 countries and use 2024 data from the Gapminder website.

 I individually analyzed each dataset, them merged them for more comprehensive analysis. Initially, my hypothesis was that GDP and population would be the strongest indicators for country selection. Though, they ended up being relatively poor predictors. The top countries with respect to Gross Domestic Product and population were Brazil and Mexico. However, they both fell into the 8th and 9th place spots out of the 14 countries for daily income and daily sugar intake. As a dessert company, both of those indicators are critical for success.

 My conclusion is the top three countries most likely to yield success are Canada, Ireland and Australia with Canada as the clear winner.

 My recommendation is to chose Canada as the first country for expansion and do further analysis to determine which metropolitan area would be best.
