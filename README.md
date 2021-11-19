# SentimentAnalysisProject
![Rich Twitter Bird](https://edlatimore.com/uploads/thumbnails/buy-retweets-ed-latimore.jpeg)

## Project Overview
For this project, we used advanced supervised modeling process and natural language processing to solve a tweet sentiment classification problem using an advanced dataset.

## Data Overview
The dataset comes from CrowdFlower via data.world. Human raters rated the sentiment in over 9,000 Tweets as positive, negative, or neither. The tweets included are sent out during the South by South West conference, mostly about Google and Apple products that was put together in 2013.

## Methodology
NLP:
- To prepare this data for modeling we decided to utilize natural language processing techniques such as removing NLTK’s stopwords, mentions (@username), the hashtag symbol (#), hyperlinks, html formatting, and non-English characters and the two most popular words, “SXSW” and “link”. Furthermore, we transformed the words into lower case, lemmatized and tokenized the words to develop a more accurate accounting of words for analysis. To vectorize the data set for modeling we used Sci-Kit Learn’s Term Frequency, Inverse Document Frequency (TF-IDF) and CountVectorizer packages. 

Modeling:
- For modeling techniques, we used Sci-Kit Learn’s Logistic Regression, with Primary Component Analysis(limits multicollinearity), Multinomial Naïve Bayes(good for text classification), Random Forest(more advanced algorithm) libraries and Keras’s Sequential neural network builder(Deep learning algorithm). We adjusted the max document frequency, min document frequency and max features hyperparameters for TF-IDF. We adjusted the Laplace smoothing alpha in the Multinomial Naïve Bayes Model. In the Neural Network, we added two hidden layers, two dropout sets and regularized the hidden layers’ weights, biases, and activation functions. We decided to use a TF-IDF tuned Multinomial Naïve Bayes Model because the model was not over fit and had a lower computational cost than the other models.

## Model Result
We are able to achieve 71% accuracy on both training data and testing data on both our naive bayes and neural network models without overfitting. However, naive bayes requires significantly less computational power so we decide to use naive bayes as our final model.
![Confusion Matrix](desktop/Screen Shot 2021-11-18 at 11.43.48 AM)


## Next Steps



## Authors
- Ely Lin
- Garrett Williams
- Dave McKinley

## Repository Navigation
```
├── notebooks
│         ├──Dave
│         ├──Ely
│         └──Garrett
├── README.md
├── presentation.pdf
└── SentimentAnalysis.ipynb
```
