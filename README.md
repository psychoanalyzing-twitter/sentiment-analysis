
# Sentiment Analysis of Tweets regarding Technology and Innovation in the UAE

This project was an assignment for our Text Analytics course @ Heriot Watt University. It looks at tweets in order to gain insights into people's views on the current state of technology, the innovations, and technological advancements made in the UAE.

## Motivation
Sentiments from Twitter could be useful for businesses and government entities.

## Method and results

### Methods 
The standard NLP workflow is abided by. What was done in each step of the workflow is briefly described below:

1. **Text-Preprocessing**. Related tweets are scraped using Tweepy.
2. **Data Labelling**. TextBlob and Vader are used to automate labelling of tweets as positive, negative, or neutral. They are then manually examined to determine which would be more accurate.
3. **Data pre-processing**. Standard pre-processing- stop words are removed, tweets are tokenized, lemmatization/stemming, ... . Lemmatization and stemming and compared against a classifier, and the best one is used in the next step. 
4. **Text Representation**. The following text representation techniques were used and compared against each other: BOW, N-grams, TF-IDF, CBOW, Skip-gram, and the pre-trained W2V model. The classifier used for comparison was the Multinomial Naive Bayes classifier, with the main metrics of comaparison precision, recall, and f1 due to class imbalance.
5. **Classification**. The best text representation models were used in a variety of classification models: LR, Facebook's FastText, and Decision Trees. 
6. **Evaluation, Visualization, and Insights**. The precision, recall, and F1 of the models are compared. Then, positive, negative and neutral tweets resulting from the best classifier are inspected.

# Results

The best performing pipeline consisted of lemmatization for the normalization of tweets, N-gram range 1 to 6 for text representation, and decision tree for classifiation, resulting in weighted prec and recall of .85 and weighted F1 of .84.


## Libraries Used
Tweepy Vader TextBlob SkLearn NLTK Numpy Pandas Gensim FastText MatPlotLib PyLDAvis

## Running instructions

A Twitter Developer account will have to be created in order to retrieve authentication keys to scrape tweets. 

To run the project, simply fork it, plug in the authentication credentials from your the Twitter Dev account into the 'Scraping Tweets' section and run the notebook.


## About
Contributors: Alora Tabuco, Bhavika Kaliya, Andrea Nabua


Task Distribution:
| Member| Tasks |
|---|---|
|Bhavika | Data Cleaning and Preprocessing, Logistic Regression, Visualization |,
|Alora|  Data Labelling and Cleaning, FastText, Decision Trees and Conclusions |,
|Andrea| Project Overview, Tweet Scraping, Text Representation|
