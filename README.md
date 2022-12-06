![Logonetflix](https://user-images.githubusercontent.com/13074725/206051218-b154735e-768e-4273-8d5a-69201dbd7df4.png)


# **<span style="color:#023e8a;font-size:200%"><center>Analysis of Netflix Content Library</center></span>**

## <center>By: Bhagirath Bhardwaj, Jinisha Kande, Paulin Jesintha Mariadoss, Renata Halim, Sohil Jain, and Sonal Kaur</center>

# **<span id="Project-Overview" style="color:#023e8a;">Project and Dataset Overview</span>**

**Netflix Content Analysis**

Netflix is known to be one of the best internet media and entertainment streaming companies. Over the years, it has faced several challenges and overcome a shift in demographics, changing viewership styles and choices. 

Netflix’s content library and its recommendations engine play a big role in influencing the content consumed by people worldwide. Research from Netflix shares that over 80% of the content watched on their platform came from their recommendations engine. 

While Netflix has enjoyed a long period of success as the sole pioneer of the internet media streaming industry, **things have changed**. There is fierce competition in the market such as `Disney+`, `Amazon Prime Video`, `HBO Max`, and others. 

In addition, Netflix is facing trouble in holding on to the content that people watch and enjoy as they are licensed under the other streaming platforms. 

>  Tip! Use the Table of Contents to browse the notebook

# **<span id="Motivation" style="color:#023e8a;">Motivation</span>**

**Our team act as hypothetical analysts working at Netflix, who have been tasked by their manager to -**

* Review all available datasets,
* Visualize them, 
* Study the changes in Netflix’s content strategy over the years and lastly,
* Come with top 3 recommendations that could be inferred.

# **<span id="summary" style="color:#023e8a;">Report Summary</span>**

## **Report Findings**

The report has a couple of findings that are discussed in depth in the conclusion section. The key findings are -

*   Netflix has been investing more in TV shows than movies over the years.
*   Netflix focuses on producing content in English, followed by Spanish and Japanese.
*   Netflix focuses on producing content in the US, followed by India and the UK.
*   Netflix generally produces content in the genres of Drama, Comedy, and Documentary.
*   Netflix has been producing more content in the last 5 years than in the previous 5 years.
*   Netflix stock price has been increasing over the years. However, the stock price has been decreasing since the start of 2020 due to the COVID-19 pandemic and rising competition from other streaming platforms such as Disney+ and Amazon Prime Video.
*   Netflix subscribers have been increasing over the years. However, the number of subscribers has been decreasing since the start of 2020 due to the COVID-19 pandemic and rising competition from other streaming platforms such as Disney+ and Amazon Prime Video.
*   Netflix has to change its stance on ad-supported content to increase its subscriber base and revenue.

## **Report Recommendation Summary**

The report finds the following top three recommendations from its analysis - 

*  Producing more Netflix Originals content
*  Create an Ad-supported subscription model
*  Capitalize more on the existing subscriber base

Our dataset was captured using a combination of tools and methods; scraping, API calls, and manual validation. Using these techniques, the author of the original dataset, Shivam Bansal, was able to capture information on a myriad of topics, namely on Netflix shows, movie titles, directors, casts, countries, release dates, ratings, and more. 

In total, our main dataset has `12` columns and `8807` rows.

**Sources** -

1.   [Netflix-Shows by Shivam Bansal](https://www.kaggle.com/datasets/shivamb/netflix-shows)

>  [Clarification of Source of dataset by Author](https://twitter.com/shivamshaz/status/1452642649442172931?s=20&t=OSh8EM8VNMZhmXSi6aBgtA)

---

In addition, the team scraped the following sources to get - 

* Netflix and other companies Stock Information using `yFinance` API
* Netflix Subscriber Count per Region and Quarters
* Netflix Subscriber Count per Country and Population
* Netflix Originals Programming Scraped Data-set


**Sources** -
2. [yFinance API - Market Data from finance.yahoo.com](https://finance.yahoo.com/)
3. [Scraped Data - Netflix Original Programming](https://en.wikipedia.org/wiki/List_of_ended_Netflix_original_programming)
4. [Scraped Data - Netflix Subscriber Count per Region and Quarters](https://www.comparitech.com/tv-streaming/netflix-subscribers/)
5. [Scraped Data - Netflix Subscriber Count per Country and Population](https://www.comparitech.com/tv-streaming/netflix-subscribers/)
6. [Scraped Data - Netflix vs Disney+ Subscriber Count](https://atlas.jifo.co/api/connectors/353c6973-eb8f-483a-a56b-598111522757)

## Dataset Descriptions

In this project we utlize multiple datasets, a brief summary of all of them are as follows:

| Dataframe Name     | Brief Description |
| ----------- | ----------- |
| `netflix_ds` | Dataset containing a list of all tv shows and movies hosted on Netflix over the years.       |
| `netflix_originals_drama_ds`   | Dataset scraped from Wikipedia for all |**Drama** Genre Shows **produced** by Netflix as a "Netflix Originals".|
| `faang` | `META`,`AMZN`,`NFLX`,`GOOG`,`AAPL` stock data from yFinance API |
| `revenue_growth_ds` | `NFLX` revenue growth from 2011-2022 per Quarter |
| `subscriber_growth` | Netflix vs Disney+ Subscriber Growth Count |
` subscriber_growth_region` | Netflix Subscriber Growth per Region and Quarter from `2018`. |
| `population_subscribers` | Netflix Subscriber Count per Country and Population.     |
