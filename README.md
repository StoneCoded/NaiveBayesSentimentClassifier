### Table of Contents

 1. Installation
 2. Motivation
 3. File Descriptions
 4. Results
 5. Licensing, Authors, and Acknowledgements

## 1. Installation.

Other than the standard Anaconda distribution of Python 3 you will also need SKLearn which documentation can be found [here](https://scikit-learn.org/stable/install.html)

## 2. Motivation

I wanted to create a simple classifier based soley from text vector counts. Ideally, the Sentiment140 Dataset from Kaggle has 1.6 million tweets with sentiment labels already attached. So using this dataset I set about creating my classifier.

## 3. File Descriptions

`Twitter Sentiment Classifier.ipynb`

This classifies sentiment in given text based from the tweets in Sentiment140.

This is pretty standard Multinomial Naive Bayes implementation. First splitting the data into labels and a training list of tweets. After this it creates vector counts of tweets before making predicitons. It includes a cell at the bottom to test custom text.

Each is commented through to aid reading and understanding.

## 4. Results

I was hoping for Positive, negative and neutral but straight away I noticed there was no neutral sentiment values existing in the dataset despite being mentioned. An accuracy of 78% was found from using MultinomialNB was observed. By testing out custom text along with browsing the initial dataset I noticed an easy way to trip up the classifier was using mixed sentiment sentences.

For example, when given :"I am very happy, not sad in any way" predicts that it is a negative sentiment. There is evidence to suggest that the dataset also struggled with this. For example the tweet; "@Viennah Yay! I'm happy for you with your job! But that also means less time for me and you..." again with mixed sentimental words is classified as negative.

This suggests a lean toward negative sentiment though more exploring of the dataset would need to be done to confirm this

## 5. Licensing, Authors, and Acknowledgements

All data was published on Kaggle [Here](https://www.kaggle.com/kazanova/sentiment140) where all licensing and gathering documentation can be found.

Feeling free to use and abuse the code above to you hearts content.
 

