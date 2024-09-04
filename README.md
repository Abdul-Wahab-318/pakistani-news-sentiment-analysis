# Sentiment Analysis on Pakistani News Articles
This project involves performing sentiment analysis on Pakistani news articles collected over the past month (August-September 2024). The primary goal is to understand public sentiment regarding various topics and events covered in the news. A total of 800+ articles were scraped from multiple news sources, and the sentiment of each article was analyzed and was given a compound score.

## Table of Contents
1. [Introduction](#introduction)
2. [Data Collection](#data-collection)
3. [Data Preprocessing](#data-preprocessing)
4. [Sentiment Analysis](#sentiment-analysis)
5. [Identifying the most common topics using Named Entity Recognition](#named-entity-recognition)
6. [Results](#results)
7. [Conclusion](#conclusion)

## Introduction
The project aims to analyze the sentiment of news articles published in Pakistan to gain insights into public opinion on various issues. This analysis can help in understanding the media narrative and public mood over the past month.

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
- **Approach:** The sentiment analysis was performed using the `VADER` sentiment analysis tool, which is well-suited for analyzing social media text and news articles.
- **Sentiment score:** Each article was given a compound score using vader.polarity_scores.
- **Challenges:** Some challenges faced included handling mixed-language text and dealing with articles that had ambiguous sentiments.

## Results
- **Summary:** After grouping the articles by the date published , it was seen that out of all the days , only two days (11-8-24 and 14-8-24) had mean positive sentiment score.
- **Visualizations:** The sentiment distribution over time was visualized using bar charts and line graphs.
- **Insights:** It was observed that the sentiments skewed heavily towards the negative side.

## Conclusion
This analysis provides a snapshot of public sentiment as reflected in Pakistani news articles. The results can be used to understand how different events influence public opinion.

