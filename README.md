# NlP Homework 12

# Warning: This Jupyter Notebook attached to this homework in extensively long because I read in the entire text of the article using the url, not just the abbreviated text provided by News API.

## News Headlines Sentiment

In this section we used the News API to call in artilce information for the most recent news associated with bitcoin and euthereum. This data pull, however, only provided us with an abbreviated version of the content of the article. To get the full article, I created a function (text_scrapper) that leveraged the url provided by the API to get the content of the article. Using this function, we were able to save the full text information, and other aspects of the article, in a DataFrame. 

Using this DataFrame, we were able to conduct sentiment analysis on the text of the articles using the SentimentIntensityAnalyzer() function and ammending the DataFrame to contain these scores. 

We were then able to determine that ethereum has a slightly higher mean positive score with 0.0967 compared to the 0.0935 score for bitcoin. Ethereum had the highest compound score with 0.999 when compared to Bitcoin, which maxed out slightly behind at 0.998. Ethereum also had the highest positive score with a 0.217.

## Tokenizer

In this section we first had to set the stop words function to the english setting, and add any superfluous, non-analytical words that we would want to ignore for subsequent analysis. Incorporating this function, as well as regex to ignore all punctuations in the text, we were able to build a tokenizer function to tokenize the text for each of the news artilces previous stored in the DataFrames. 

## NGrams and Frequency Analysis

After tokenizing the text above, we then used the nltk libary to apply the ngrams function to the text. This allowed us to find the most frequently occuring group of words, with a group frequency of 2. 

## Word Clouds

Similar to the ngrams section, the word clouds section allows us to visualize the most frequently occuring, and theoretically most important, words by plotting them in a diagram where size is directly proportional to frequency. 

## Named Entity Recognition

After concatenating the text for each of the articles for the individual crypto currencies, we were then able to apply the name entity recognition platform from the spacy library to identify the places, organizations and people, among other classifications, in the text.

