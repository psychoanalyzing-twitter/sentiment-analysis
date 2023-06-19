
# Sentiment Analysis of Tweets regarding Technology and Innovation in the UAE

A project which was an assignment for our Text Analytics course @ Heriot Watt Uni. This project looks at Tweets in order to gain insights into people's views on the current state of technology, the innovations, and technological advancements made in the UAE.

## Motivation

Motivate your research question or business problem. Clearly explain which problem is solved.

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

The best performing pipeline was 


## Repository overview

Provide an overview of the directory structure and files, for example:

├── README.md
├── data
├── gen
│   ├── analysis
│   ├── data-preparation
│   └── paper
└── src
    ├── analysis
    ├── data-preparation
    └── paper

## Libraries Used

## Running instructions

Explain to potential users how to run/replicate your workflow. If necessary, touch upon the required input data, which secret credentials are required (and how to obtain them), which software tools are needed to run the workflow (including links to the installation instructions), and how to run the workflow.


## More resources

Point interested users to any related literature and/or documentation.


## About
Contributors: 


Task Distribution:

