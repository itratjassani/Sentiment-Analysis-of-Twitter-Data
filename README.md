# Sentiment Analysis of Twitter Data Project

## Problem Statement

The most important or the most precious assets of any organization, company, firm, etc. are its customers. And what makes a customer brand loyal is when he/she gets what he wants from the respected organization.

A person can predict someone’s mood by their verbal or non-verbal communication (facial expressions) but how it can be possible that we can predict our customers' sentiments live while chatting?

## What is Sentiment Analysis

This is where Semantic Analysis comes in, the idea of the project is that users can know the mood of the sender of the message which can be positive, negative, or neutral, and also the magnitude of it. Just imagine how productive it can be the customer service.

The goal of Sentiment Analysis is to determine the attitude of the masses towards the subject of interest.

It is the classification of the polarity of a given text in the document, sentence, or phrase.

## Why Sentiment Analysis is important?

* Is this product review is positive or negative?
* Is this customer email satisfied or dissatisfied?
* Based on a sample of tweets, how are people responding to this ad campaign/product           release/news item?
* How have blogger’s attitudes about the president changed since the election?

## Why Twitter data for sentiment Analysis

* Popular microblogging site.
* Short text messages of 140 characters.
* 240+ million active users.
* 5 million tweets are generated every day.
* Twitter's audience varies from the common man to celebrities.
* Users often discuss current affairs and share personal views on various objects.
* Tweets are small in length and hence unambiguous.

## Challenges

* People express opinions in complex ways.
* In Opinion texts, lexical content alone can be misleading.
* Unstructured and non-grammatical.
* Out of vocabulary words.
* Extensive usage of acronyms like asap, lol.
* Timely results so that the user can reply as soon as possible.
* Achieving accuracy as the user’s reply depends on the results shown by the software.

## Process Flow

![image](https://github.com/itratjassani/Sentiment-Analysis-of-Twitter-Data-Project/assets/35358807/840e97e4-1560-4955-9bb5-ce160cc44429)

## Approach
### Tweet Dataset
* Downloaded the Twitter dataset from NLTK libraries.
* We have 10K rows for Positive and negative tweets, 5K for each.
### Tokenization
* Downloaded the Twitter dataset from NLTK libraries.
* We have 10K rows for Positive and negative tweets, 5K for each.
### PreProcessing
* Non-English tweets removed.
* Remove the URL links, hashtags, target mentions, and numbers.
* Neglect Empty Column N/A
* Expand Contraction.
* Stemming & Lemmatization - Change the verbs to their first form.
* Replace sequence of repeated characters e.g.: “coooooool”.
* Remove Nouns and prepositions.
### Feature Extraction
* Word polarity score using Wordnet. 
* Positive/Negative/Extremely Positive/Extremely Negative Emoticons.
* The number of special characters, POS.
### Classifier and Prediction 
* The features extracted are passed on to the naive Bayes classifier.
* The model built is used to predict the sentiment of the tweets.
* We have used 70% data for training and 30% of the data for testing.
### Principle of Naive Bayes Classifier
A Naive Bayes classifier is a probabilistic machine learning model that’s used for classification tasks. The crux of the classifier is based on the Bayes theorem.

* ![image](https://github.com/itratjassani/Sentiment-Analysis-of-Twitter-Data-Project/assets/35358807/456b1aff-245e-4947-a39f-c3d0788785ec)
  
Using Bayes theorem, we can find the probability of A happening, given that B has occurred. Here, B is the evidence and A is the hypothesis. The assumption made here is that the predictors/features are independent. That is presence of one particular feature does not affect the other. Hence it is called naive.

## Results (Qualitative Evaluation)
![image](https://github.com/itratjassani/Sentiment-Analysis-of-Twitter-Data-Project/assets/35358807/57b5cf25-4bbc-4fda-9dbe-3077ff8b019b)

## Conclusion 
* Evaluating the classification accuracy of the predictions from the model confirms that the model performs as expected, achieving a score of 99%.
* We conclude that using different NLTK classifiers it is easier to classify the tweets and the more we improve the training data set more we can get accurate results.
* For our feature-based approach, feature analysis reveals that the most important features are those that combine the prior polarity of words and their parts of speech tags.
* There is always a scope for increasing the accuracy by extracting more features that are relevant  to the sentiments.









