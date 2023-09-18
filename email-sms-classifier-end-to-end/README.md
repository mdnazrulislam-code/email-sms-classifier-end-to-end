
Spam Email / Sms detection using Multinomial Naive Bayes 

Problem:
	Identifying and distinguishing spam messages and emails using the Multinomial Naïve Bayes model.

What are Multinomial Naive Bayes? 
	Multinomial Naive Bayes is one of the most popular supervised learning classifications that is used for the analysis of categorical text data. Text data classification is gaining popularity because there is an enormous amount of information available in email, documents, websites, etc. that needs to be analyzed.

In statistics, Naive Bayes classifiers are a family of simple "probabilistic classifiers" based on applying Bayes' theorem with strong (naive) independence assumptions between the features. At the time of writing this repository, there are 5 different types of Naive Bayes classifiers, which as follow:

 Bernoulli Naive Bayes classifier
Categorical Naive Bayes classifier
Complement Naive Bayes classifier
Gaussian Naive Bayes classifier
Multinomial Naive Bayes classifier


In this project, I  have used the Multinomial Naive Bayes classifier to detect spam messages, the reason for using this classifier is the simple implementation, high accuracy, and vector implementation method of this model. It should be noted that other methods can also be used to detect spam messages, such as the Complement Naive Bayes classifier and Tf-Idf.


Explanation of Multinomial Naive Bayes 👍
	Multinomial Naive Bayes  implements the naive Bayes algorithm for Multinomial distributed data, and is one of the two classic naive 
Bayes variants used in text classification (where the data are typically represented as word vector counts, although tf-idf vectors are also known to work well in practice). 
The distribution is parametrized by vectors θ y = ( θ y 1 , … , θ y n ) for each class y where n is the number of features (in text classification, the size of the vocabulary) and θ y i is the probability P ( x i ∣ y ) of feature i appearing in a sample belonging to class y

The parameters θ y is estimated by a smoothed version of maximum likelihood, i.e. relative frequency counting:
θ ^ y i = N y i + α / N y + α nwhere N y i = ∑ x ∈ T x i is the number of times feature i appears in a sample of class y in the training set T and N y = ∑ i = 1 n N y i is the total count of all features for class y

Dataset used :  
	I used the smsSpamCollection dataset to train my model, which can be accessed via the link below:
    https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset

Relation between Spam(1) and Ham(0):











	
Model Building Steps:

 Import libraries
 Upload dataset
 Create the data frame
 Split the data
 Vectorize the data
 Train & predict
 calculate accuracy, precision, and recall
 calculate the confusion matrix
 Test the model with a new Sms/Email message
Export Model
Create web app (streamlit)
Deploy into Heroku

