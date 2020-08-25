# Depression-Detection-using-Text-Analysis
MDD, also commonly referred to as Clinical Depression, is considered as the most typical form of the disease. MDD can be diagnosed by the presence of two symptoms namely being depressed most of the day or markedly diminished interest or pleasure. Some more common symptoms of depression are retardation almost every day, fatigue or loss of energy almost every day, feelings of worthlessness or excessive guilt, diminished ability to concentrate or indecisiveness almost every day, recurrent thoughts of death or suicidal ideation.
Depression Detection through Text Analysis

In this we aimed at detecting whether the person is depressed or not via social media. These days people are very active on online platforms such as Twitter and usually express their thoughts through messages and blogs they most. Therefore, we considered this data generated as a source for analysing the presence of depression in them. It was implemented in following phases:

•	Data Collection: The dataset has been generated combining part of the Sentiment140 [6] (8,000 positive tweets), and another one for depressive tweets (2,314 tweets), with a total of 10,314 tweets. The Sentiment140 dataset contains 1,600,000 tweets extracted using the twitter API. The tweets have been annotated (0 = negative, 2 = neutral, 4 = positive) and they can be used to detect sentiment. It contains the following 6 fields:
target: the polarity of the tweet (0 = negative, 2 = neutral, 4 = positive)
ids: The id of the tweet (2087)
date: the date of the tweet (Sat May 16 23:58:44 UTC 2009)
flag: The query. If there is no query, then this value is NO_QUERY.
user: the user that tweeted.
text: the text of the tweet.

For our experiment, we have taken a sample of 8,000 tweets with polarity of 4, the positive ones. Depressive Tweets have been Web scraped with TWINT [7]. The entire data has been extracted from [8]. The final dataset has three attributes tweet-id, tweet content and label that is 0 or 1 depending on whether the tweet is positive or negative respectively.

•	Word-Cloud Analysis: A word-cloud is created using the python in-built function for depressive and positive words by including all the words present in tweets with label 1 and label 0 respectively.

•	Data Pre-processing: Data pre-processing has been done for stemming and removing stop words and then tokenizing the tweets by using whitespace as the delimiter. As the keyword matching strategy is widely used, words must have unified representations regardless of the tense and voice. For example-―marrying and ―married should be represented as ―marri uniformly. For the purpose of stemming porter stemming algorithm has been used.
                                              				5

•	Classification: Using Bayes theorem for analysing if a person writing a particular tweet can be diagnosed with depression or not. The probabilities have been calculated using the probability of each word in a tweet to belong to a particular category and then multiple importance of word.

