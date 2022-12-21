# Election_analysis

The purpose of this project is to perform a data analysis on the upcoming presidential election in nigeria. The main point of focus is analyzing historical election data, perform sentiment anaysis on tweets and nairaland ( A popular nigerian website) and explore the curiosity of people on their most preferred candidates.

## Approach 

This project was approached by analyzing the front runners for the upcoming election on the aforementioned plaforms

In the Jupyter Notebook, you will leearn how I carried out the following steps for the project:

1. Import Libraries
2. Data Gathering (web scraping (nairaland), web automation (tweet mining using SNScrape library) and manually downloading data)
3. Data Cleaning (Tweets processing, location and mention cleaning, quality and tidiness cleaning)
4. Data Exploration
5. Sentiment Analysis

## Tweets Processing Steps
To reach the ultimate goal, there was a need to clean up the individual tweets. To make this easy, I created a function "cleanTxt" in my Python program which I further applied to the "Tweets" to produce the desired results. This user-defined function was used to remove punctuations, links, emojis, and stop words from the tweets in a single run. Additionally, I used a concept known as "Tokenization" in NLP. It is a method of splitting a sentence into smaller units called "tokens" to remove unnecessary elements. Another processing done is the removal of stop words. Stop words are a set of commonly used words in any language. For example, in English, “the”, “is” and “and”, are stop words.

## Sentiment Analysis
For this analysis, I went with TextBlob. Text Blob analyzes sentences by giving each tweet a Subjectivity and Polarity score.  Based on the Polarity scores, one can define which tweets were Positive, Negative, or Neutral. A Polarity score of < 0 is Negative, 0 is Neutral while > 0 is Positive. I used the "apply" method on the "Polarity" column in my data frame to return the respective Sentiment Category.
