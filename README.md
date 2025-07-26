Overview

This project is an Email/SMS Spam Classifier that uses machine learning to distinguish between spam ("junk") and ham ("legitimate") messages. The classifier is trained on a dataset of 5,169 text messages, achieving high accuracy in identifying spam while minimizing false positives.
Key Features

Text Preprocessing: Cleans and normalizes text data through:
Lowercasing
Tokenization
Special character removal
Stopword removal
Stemming (Porter Stemmer)

Exploratory Data Analysis:

Visualizations of message length distributions (characters, words, sentences)
Word frequency analysis for spam vs. ham
Hypothesis testing confirming spam messages are significantly longer

Machine Learning Models:

Tested 8 classifiers including Naive Bayes variants, SVM, Logistic Regression, and Random Forest
Bernoulli Naive Bayes selected as best model with:

96.6% accuracy

96.6% precision (critical for minimizing false spam flags)

Technical Details
Data:

Original dataset: 5,572 messages (spam.csv)

After cleaning: 5,169 messages (87.4% ham, 12.6% spam)

Feature Engineering:

CountVectorizer for text-to-numeric conversion

Added features: character count, word count, sentence count

Performance Metrics:

text
Best Models:
1. MultinomialNB - 97.4% accuracy, 88.8% precision
2. BernoulliNB - 96.6% accuracy, 96.6% precision 
3. Logistic Regression - 97.1% accuracy, 94.6% precision
How to Use
Requirements:

Python 3.x

Libraries: pandas, numpy, scikit-learn, nltk, matplotlib, seaborn


