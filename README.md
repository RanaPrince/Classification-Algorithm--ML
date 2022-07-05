# Classification-Algorithm--ML
Use of Machine Learning ALgorithms for Classification:

- Gradient Boosted Decision Tree
- Descision Tree
- Logistic Regression


On the Kaggle problem for Donors choose Data, Gradient Boosted Descision Trees are used for the best efficiency and performance metrics.


Data From : [https://www.kaggle.com/c/donorschoose-application-screening]


Also various featurization NLP methods are used like:

- Word2vec
- tfidf
- tfidf Word2Vec

Used 3 algorithms here to counter the Classification problem:

- Logistic Regression
- Descision Trees
- Gradient Boosted Descision Trees

**Cross Validation**
(Cross-validation is a technique for determining the best parameter values before we set the final for out model training by training it on the subset of input data and testing on previously unseen subset of the input data)

- Grid Search CV
- Random Search CV


**For Descision Trees and Logistic Regression**

Here we see that the test AUC for tfidf & TF-iDF W2V features is nearly same.The tfidf is better than tfidfW2V by a slight margin. When we use the important features with non-zero feature importance we get a better AUC with Logistic Regression.

**For GBDT:**

Here we see that the train AUC for tfidf & TF-iDF W2V features is nearly same but there's a difference while the Test data comes to play. The tfidf is better than tfidfW2V by a slight margin.The GBDT also performs better than descision trees evident from our performance scores in previous assignments.

Also, here we've used LightGBM reason being, Faster training speed and higher efficiency: Light GBM use histogram based algorithm i.e it buckets continuous feature values into discrete bins which fasten the training procedure.(Src:Google)

So,eventually testing for different sets of features always backs our selection criteria for which features,featurizations to consider.
