# Sentiment Analysis on Pakistani News Articles
This project involves performing sentiment analysis on Pakistani news articles collected over the past month (August-September 2024). The primary goal is to understand media coverage regarding various topics and events covered in the news. A total of 800+ articles were scraped from multiple news sources, and the sentiment of each article was analyzed and was given a compound score.

## Table of Contents
1. [Introduction](#introduction)
2. [Data Collection](#data-collection)
3. [Data Preprocessing](#data-preprocessing)
4. [Sentiment Analysis](#sentiment-analysis)
5. [Identifying the most common topics using Named Entity Recognition](#named-entity-recognition)
6. [Results](#results)
7. [Conclusion](#conclusion)

## Introduction
The project aims to analyze the sentiment of news articles published in Pakistan to gain insights into what is happening in the country. This analysis can help in understanding the media narrative over the past month.

## Data Collection
- **Web Scraping:** The data was collected using web scraping techniques, leveraging libraries such as `BeautifulSoup` and `requests`.
- **Sources:** Articles were scraped from multiple popular Pakistani news websites: Geo news , Dawn news and The news International.
- **Data:** The dataset consists of 800+ articles that are related to pakistan or pakistani politics.

## Data Preprocessing
- **Text Cleaning:** Removed HTML tags, special characters, and unnecessary whitespace from the text.

## Sentiment Analysis
- **Approach:** The sentiment analysis was performed using the `VADER` sentiment analysis tool, which is well-suited for analyzing social media text and news articles.
- **Sentiment score:** Each article was given a compound score using vader.polarity_scores.
- **Challenges:** Some challenges faced included handling mixed-language text and dealing with articles that had ambiguous sentiments.

## Identifying the most common topics using Named Entity Recognition
- **Approach:** The Named Entity Recognition (NER) was done using `Spacy` loaded with `en_core_web_sm` 
- **NER Labels:** Each article's title was scanned for entites which were then kept track of using the Counter collection.

## Results
- **Summary:** After grouping the articles by the date published , it was seen that out of all the days , only two days (11-8-24 and 14-8-24) had mean positive sentiment score.
- **Visualizations:** The sentiment distribution over time was visualized using bar charts and line graphs.
- **Insights:** It was observed that the sentiments skewed heavily towards the negative side. The most common entities in the news were Karachi , Pakistan , PTI and Balochistan in the mentioned order. This is probably due to the influx of news articles related to the cyclone closing in on Karachi , political instability due to conflict between government and opposition parties and the recent terrorist attacks in Balochistan

![Sentiment Analysis Chart](/sentiment_analysis_chart.png)
![NER-Chart](/ner_chart.png)

## Conclusion
This analysis provides a snapshot of the media coverage on the news. The results can be used to understand how different events influence public opinion. The consistently negative sentiments of the news can negatively influence the public, making them believe that there is no hope. It is necessary for us to stop and think for a moment and look at the bigger picture before forming any opinions. If we are constantly fed negative news then our beliefs will be negative as well. This is why it is important for us to pay close attention to what information we are consuming becasue it can subconsciously influence our thinking. 

