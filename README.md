# Amazon_Food_Reviews_Model_Deployment

![Amazon_Food_Reviews](https://miro.medium.com/max/523/1*bXDiOoCFTSJJdTQ7JbuijQ.png)

##  Amazon_Food_Reviews_Featurization

### First We want to know What is Amazon Fine Food Review Analysis?
This dataset consists of reviews of fine foods from amazon. The data span a period of more than 10 years, including all ~500,000 reviews up to October 2012. Reviews include product and user information, ratings, and a plaintext review. We also have reviews from all other Amazon categories.

Amazon reviews are often the most publicly visible reviews of consumer products. As a frequent Amazon user, I was interested in examining the structure of a large database of Amazon reviews and visualizing this information so as to be a smarter consumer and reviewer.

Source: https://www.kaggle.com/snap/amazon-fine-food-reviews

### Introduction

The Amazon Fine Food Reviews dataset consists of reviews of fine foods from Amazon.

1. Number of reviews: 568,454
2. Number of users: 256,059
3. Number of products: 74,258
4. Timespan: Oct 1999 — Oct 2012
5. Number of Attributes/Columns in data: 10

### Attribute Information:
1. Id
2. ProductId — unique identifier for the product
3. UserId — unqiue identifier for the user
4. ProfileName
5. Helpfulness Numerator — number of users who found the review helpful
6. HelpfullnessDenominator — number of users who indicated whether they found the review helpful or not
7. Score — rating between 1 and 5
8. Time — timestamp for the review
9. Summary — brief summary of the review
10. Text — text of the review

## Objective
Given a review, determine whether the review is positive (Rating of 4 or 5) or negative (rating of 1 or 2).

[Q] How to determine if a review is positive or negative?

[Ans] We could use the Score/Rating. A rating of 4 or 5 could be cosnidered a positive review. A review of 1 or 2 could be considered negative. A review of 3 is nuetral and ignored. This is an approximate and proxy way of determining the polarity (positivity/negativity) of a review.

To Know the Complete overview of the Amazon Food review dataset and Featurization visit my [medium blog](https://medium.com/analytics-vidhya/amazon-fine-food-reviews-featurization-with-natural-language-processing-a386b0317f56)

##   Trained the model by NaiveBayes algorithm 

![Naive_bayes](https://cdn.educba.com/academy/wp-content/uploads/2019/04/Naive-Bayes-Algorithm.jpg)

### Applied Multinomial NaiveBayes on these feature sets
- Review text, preprocessed one converted into vectors using (TFIDF)

Naive Bayes is a statistical classification technique based on Bayes Theorem. It is one of the simplest supervised learning algorithms. Naive Bayes classifier is a fast, accurate, and reliable algorithm. Naive Bayes classifiers have high accuracy and speed on large datasets.

Naive Bayes is the most straightforward and fast classification algorithm, which is suitable for a large chunk of data. Naive Bayes classifier is successfully used in various applications such as spam filtering, text classification, sentiment analysis, and recommender systems. It uses Bayes theorem of probability for prediction of unknown class.

Naive Bayes makes an assumption that features are conditionally independent. Theoretically, if the assumption does not hold true then the performance of NB degrades. But the research has shown that even if there is some feature dependency the Naive Bayes gives the best result.

To Know detailed information about NaiveBayes algorithm and implementation  please visit my [Medium blog](https://medium.com/analytics-vidhya/naive-bayes-algorithm-with-amazon-food-reviews-analysis-66bb59b66e62)


## Amazon_Food_Reviews_Model_Deployment

![Untitled](https://user-images.githubusercontent.com/67965686/101061971-1571d100-35b7-11eb-8136-1a7268e829b7.png)

Building a machine learning project is one thing but what matters at the end is how you show your project to the world. Documenting your whole project on GitHub is another thing but deploying your deep learning model as a web application is totally different gameball.

In order for Machine Learning Engineers to succeed at work, they need to build services such that other teams can use or a product where people can use it directly. Essentially, the goal is to provide a model as a service and for that there is a concept called API. API is the way for computer systems to talk to each other over Internet Protocols. They act as an agent which takes information from the user to the server and then again from server to the user giving back the answer. Flask provides that capability. Flask will act as an API between your model and the HTML file.

We begin by creating a project folder where we define all dependencies in the requirements.txt file. To ensure that all dependencies are isolated from our application, we create a virtual environment for our working space.

To deploy we want to train our model and save the outputs in a pickle file and these pickle files are used for predict the new reiews in production.

### Steps

- Create GitHub Repository (optional)
- Create and Pickle a Model Using Titanic Data.
- Create Flask App.
- Test Flask App Locally (optional)
- Deploy to Heroku.
- Test Working App.

### Results

###### Positive Reviews

![Untitled](https://user-images.githubusercontent.com/67965686/101115763-e173cb80-3609-11eb-9bab-b3dff29bb8e2.png)

###### Negative Reviews

![Untitled](https://user-images.githubusercontent.com/67965686/101117332-c5bdf480-360c-11eb-8b9b-7f6090eb324d.png)

I am deployed app in Heroku Platform to see visit [here](https://amazon-food-review-analyzer.herokuapp.com/)

###### Thanks for reading and your patience. I hope you liked the post, let me know if there are any errors in my post.

### Contact

[Email](sachin.s1dn@gmail.com)
[Linkedln](https://www.linkedin.com/in/sachin-d-n-1st-8150351b2/)
[Github](https://github.com/Sachin-D-N/Amazon_Food_Reviews)
[Medium](https://sachin-s1dn.medium.com/)
[Twitter](https://twitter.com/home)


