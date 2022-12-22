# BTC_Twitter_sentiment_analysis

The [BTC_sentiment_analysis.ipynb](https://github.com/THouwe/NLP_sentimentAnalysis_BTC_Python/blob/main/BTC_sentiment_analysis.ipynb) notebook, shows how to download and preprocess 100.000 Bitcoin (BTC) tweets from 2022-11-01 to 2022-11-15 to perform sentiment analysis to gather market intelligence. The aim of the analysis is to understand what are people’s opinions about BTC tweets.

Sentiment analysis consists of converting a text into a score that estimates its sentiment (e.g., demand for a given product) and can be deemed as a classification task (e.g., to extract subjectivity and sentiment polarity from text data).

Web scraping is done using snscrape (https://github.com/JustAnotherArchivist/snscrape). \
Filtering for English language is done using langdetect (https://github.com/Mimino666/langdetect). \
Sentiment analysis is done using spacytextblob (https://github.com/SamEdwardes/spacytextblob).

Scraped data looked like this: \
<img src="https://github.com/THouwe/NLP_sentimentAnalysis_BTC_Python/blob/main/noPreproc.JPG" width="300" height="300">

After preprocessing, including removal of symbols, URLs, and non-ASCII characters, and removal of non-English Tweets, data looked like this: \
<img src="https://github.com/THouwe/NLP_sentimentAnalysis_BTC_Python/blob/main/preproc2.JPG" width="300" height="300">


Finally, sentiment analysis is carried out.
Before analyzing the content of the tweets, Tweets underwent further preprocessing, including lemmatization (using the WordNetLemmatizer).

Scores look like this: \
<img src="https://github.com/THouwe/NLP_sentimentAnalysis_BTC_Python/blob/main/sentiment2.JPG" width="500" height="300">

<img src="https://github.com/THouwe/NLP_sentimentAnalysis_BTC_Python/blob/main/sentiment3.JPG" width="400" height="300">

Most common words in positive Tweets: \
<img src="https://github.com/THouwe/NLP_sentimentAnalysis_BTC_Python/blob/main/positiveWords.JPG" width="500" height="300">

Most common words in negative Tweets: \
<img src="https://github.com/THouwe/NLP_sentimentAnalysis_BTC_Python/blob/main/negativeWords.JPG" width="500" height="300">

**Conclusion:** According to this analysis, with a mean sentiment of 0.07 (SD = 0.22) there is a slight but prevalent positive opinion in BTC tweets.
