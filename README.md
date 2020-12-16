# NlP Homework 12

## News Headlines Sentiment

After using the NewsAPI to read in the top headlines for both Bitcoin and Ethereum we were able to read this information into a pandas DataFrame. This subsequently allowed us to conduct sentiment analysis on the text of the articles using the SentimentIntensityAnalyzer() function and ammending the DataFrame to contain these scores. 

We were then able to determine that bitcoin had a slightly higher mean positive score with 0.07 compared to the 0.04 score for ethereum. Also, ethereum had the highest compound score with 0.877 when compared to Bitcoin, which maxed out at only 0.801. Finally, ethereum also had the highest positive score with a 0.318.

## Tokenizer

In this section we first had to set the stop words function to the english setting, and add any superfluous, non-analytical words that we would want to ignore for subsequent analysis. Incorporating this function, as well as regex to ignore all punctuations in the text, we were able to build a tokenizer function to tokenize the text for each of the news artilces previous stored in the DataFrames. 

## NGrams and Frequency Analysis

After tokenizing the text above, we then used the nltk libary to apply the ngrams function to the text. This allowed us to find the most frequently occuring group of words, with a group frequency of 2. 

## Word Clouds

Similar to the ngrams section, the word clouds section allows us to visualize the most frequently occuring, and theoretically most important, words by plotting them in a diagram where size is directly proportional to frequency. 

## Named Entity Recognition

After concatenating the text for each of the articles for the individual crypto currencies, we were then able to apply the name entity recognition platform from the spacy library to identify the places, organizations and people, among other classifications, in the text.

## 