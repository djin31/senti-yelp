# Senti-Yelp
Senti-Yelp is a sentiment mining system to predict ratings given by users based on their reviews. 
We will be working with Bag-of-Words based TFIDF vector representation of reviews. Over this will use simple classifiers from `sklearn` namely: Naive Bayes, Logistic Regression and SVM.

The models and accuracies reported are after training the models on a small subset (100k examples) of Yelp reviews.

### Preprocessing
First the text is preprocessed and a TFIDF vector representation of reviews are generated. The details and implementation of preprocessing can be found in [preprocessing.ipynb](preprocessing.ipynb).

### Training Classifiers
We experiment with Multinomial Naive Bayes, Logistic Regression and LinearSVC models using the same feature vectors created during preprocessing. As has been observed often we see that accuracies of different models are in the order Naive Bayes << Logistic Regression ⩽ SVM.

| Model| Accuracy % |
| ------------- | ------------- |
| Naive Bayes | 56.00 |
| Logistic Regression | 69.22 |
| SVM | 69.24 |
