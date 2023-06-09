# CIS5190-Final-Project
### Amazon Food Review - NLP with Sentiment Analysis

### Project Overview

For this study, we conducted sentiment analysis on Amazon food review, which is a rich source of labeled data that can be used to train and test AI models for natural language processing tasks. Understanding the reviews could provide insights in customer preferences, help product recommendation and identify purchase trends. We have implemented various models including both traditional machine learning (ML) strategies and deep learning methods: Naive Bayes, Logistic Regression, XGBOOST, and LSTM. Evaluations are performed on all implemented models and hyper-parameter tuning is conducted on the one with the highest F1 score. Deep learning model LSTM with architecture of 2 LSTM layers plus one dense layer gives the best default benchmarking performance and efficacy and is then optimized by hyperparameter tuning. A tunned LSTM model using bag of words vectorized data with 64 units in each layer, learning rate = 0.002, batch size = 96, number of epochs = 3 output the best result with accuracy score of 0.93, percision score of 0.96, recall score of 0.96, and F1 score of 0.96.

### Code

The code is provided in the `Amazon_Food_Review_NLP_with_Sentiment_Analysis.ipynb` notebook file. However, the code is not displayed properly on github due to the version of Jupyter notebook that we used is the lastest version. Therefore, we also provided the link to the Colab notebook, which is [CIS 5190 Final_Project_Amazon_Food_Review_NLP_with_Sentiment_Analysis](https://colab.research.google.com/drive/1mnLsd75rRE96ucLHaNfUUfL0a_693hhZ?usp=share_link).

### To Run the Program
Connect to the Google shared drive to obtain the dataset [CIS 519 Project](https://drive.google.com/file/d/1oIclraonEC5SH5NbUXlDyTBLOsz2v5Fh/view?usp=share_link)
or you can directly download the dataset [Amazon Fine Food Review](https://www.kaggle.com/snap/amazon-fine-food-reviews) from Kaggle and upload to Colab.

### Install

The following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)
- [tensorflow](https://www.tensorflow.org/)
- [seaborn](https://seaborn.pydata.org/)
- [string](https://docs.python.org/3.5/library/string.html)
- [collections](https://docs.python.org/3.3/library/collections.html)
- [wordcloud](https://github.com/amueller/word_cloud)
- [nltk](https://www.nltk.org/)
- [keras](https://keras.io/)


### Data

The dataset contains 568,454 food reviews Amazon users left from October 1999 to October 2012.).

### Features

* Id
* ProductId: unique identifier for the product
* UserId: unique identifier for the user
* ProfileName
* HelpfulnessNumerator: number of users who found the review helpful
* HelpfulnessDenominator: number of users who indicated whether they found the review helpful Score - rating between 1 and 5
* Time: timestamp for the review
* Summary: brief summary of the review
* Text: text of the review

### Target variable
* Score: rating between 1 and 5
