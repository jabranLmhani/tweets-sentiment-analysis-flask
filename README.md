# Tweet Sentiment Analysis:
- data resource: https://www.kaggle.com/kazanova/sentiment140
- This data set contains 1.6 million tweets texts extracted using the twitter API. The tweets have been annotated (0 = negative, 4 = positive) and they can be used to detect sentiment. Goals:
Design a NLP model that is able to predict the polarity (negative or positive) of the tweet. 


# To Run the project:
- To run the project we recommend you use a virtual environment.
- You can see the app in Heroku : https://sentiment-analysis-word2vec.herokuapp.com

# Data processing:
the tasks that have been carried out in this step are :

- Removing abreviations, stop words and ponctuation 
- lemmatization  (using <code>nltk</code>)
- training our Word2Vec model on them with window size 5 and vector size 300

# Logistic Regression model:
After the last step : data processing, the following steps are: <br/>
- Representing each tweet by the sum of the vectors of each word in the tweet and we stored them into a matrix that represented our features.
- Spliting the dataset into training and testing sets with the testing set containg 30% of the data.
- Training the Logistic Regression Model.
