# Detecting-Hate-Speech


Building a basic ML model for text classification
The task is to inout data from the csv which contains tweets and a label which classifies whether it is a hate speech or not. 

Things to note
• label is the column that contains the target variable or the value that has to be predicted. 1 means it's a hate speech and 0 means it is not.
• tweet is the column that contains the text of the tweet. This is the main data on which NLP techniques will be applied.

First we do data cleaning to remove noise from the tweets like the special symbols, stopwords and unicode characters.

Then we do feature engineering to get numercial values from the clean text(tweet). The columns added are words_count(number of words in the cleaned tweet), character_count(number of characters in the cleaned tweet),isprompt(to indicate is it a question), isneg(to indicate if it contains any negative word like nor , not isn't etc.), israre(to indicate whether it contains the rare 100 words from the tweet corpus).

Once the data is ready we split it into train and test using sklearn library and then train our model.

Naive Bayes ML algorithm is used to train the model and then accuracy is used as metrics to test it.

