### Sentiment Analysis
Sentiment analysis, also known as opinion Mining is a branch of data mining where, text data is analyzed for getting emotions, beliefs, and attitudes of the public toward a particular topic, issue, product, or service. It is very helpful in understanding customer behaviour, public emotion towards a social issue, public support for a topic, etc. Here we have used a dataset of covid-19 related tweets to perform the sentiment analysis task. Using sentiment analysis the social media posts or tweets will be classified into various emotional categories. The basic classification is positive, negative, and neutral.

### Covid-19 Tweet Dataset
A publicly available datatset, which contains 44955 covid-19 related tweets is used.

### Preprocessing
Preprocessing stage include the following steps :
#### 1. Text Cleaning
Removal of stopwords, usernames, special characters and digits, also the conversion of all texts into lowercase for the uniformity. 
#### 2. Lemmatization
Reducing the words into their base form called lemma (eg : talking/talks/talked = talk)
#### 3. Sentiment Labelling
__TextBlob__ libabry in python is used assign value for tweets between -1 and +1 where, -1 is extremely negative and +1 is extremely positive. Based on the polarity values assigned two labelled datasets are created : 
* Two-class dataset : Tweets with polarity scores [-1,0] and [0,+1] are labelled as negative and positive respectively.
* Three-class dataset : Tweets with polarity scores [-1,-0.2], [-0.2,+0.2] and [+0.2,+1] are labelled as negative, neutral and positive respectively.
### Feature Extraction
Term Frequency - Inverse Document Frequency (TF-IDF) vectorizer is used to convert the textual data into numerical vectors.
### Sentiment Classification and Modelling
Three different machine learning models are used for the sentiment classification.
1. Decision Tree
2. Random Forest
3. Bidirectional Long Short-Term Memory (BiLSTM)

### Implementation
The project is implemented in python. 80% of the dataset is used for training and 20% is used for testing.

### Reference
The inspiration for doing this project is the following research paper : <br>
[A Reliable Sentiment Analysis for Classification of Tweets in Social Networks](https://rdcu.be/dJrbY) <br>
Social Network Analysis and Mining (2023), Volume 13 : Article 7

### Results and Findings

![Comparison of the performances of various learning models on two-class dataset](https://github.com/Answab/sentiment-analysis/blob/main/Graphs/2Cimage.png)




