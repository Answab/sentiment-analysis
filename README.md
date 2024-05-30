### Sentiment Analysis
Sentiment analysis, also known as opinion Mining is a branch of data mining where, text data is analyzed for getting emotions, beliefs, and attitudes of the public toward a particular topic, issue, product, or service. It is very helpful in understanding customer behaviour, public emotion towards a social issue, public support for a topic, etc. Here we have used a dataset of covid-19 related tweets to perform the sentiment analysis task. Using sentiment analysis the social media posts or tweets will be classified into various emotional categories. The basic classification is positive, negative, and neutral.

### Covid-19 Tweet Dataset
A publicly available datatset, which contains 44955 covid-19 related tweets is used

### Preprocessing
Preprocessing stage include the following steps :
#### 1. Text Cleaning
Removal of stopwords, usernames, special characters and digits, also the conversion of all texts into lowercase for the uniformity. 
#### 2. Lemmatization
Reducing the words into their base form called lemma (eg : talking/talks/talked = talk)
#### 3. Sentiment Labelling
_TextBlob_ libabry in python is used assign value for tweets between -1 and +1 where, -1 is extremely negative and +1 is extremely positive. 


