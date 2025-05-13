# Spam-Detection

NOTE : To use, change line 14 of spamdetect.py according to the location of file on your computer.

SMS Spam Detection using different ML models: Multinomial Naive Bayes, Support Vector Machine (SVM), K Nearest Neighbours (KNN)

Problem Statement: 
SMS Spam Detection using Machine Learning Approach
Short Message Service (SMS) has grown rapidly and the reduction in the cost of messaging services has resulted in growth in unsolicited commercial advertisements (spams) being sent to mobile phones. Lack of real databases for SMS spams, short length of messages and limited features, and their informal language are the factors that may cause the established email filtering algorithms to underperform in their classification. A database of real SMS Spams from UCI Machine Learning repository is used, and after preprocessing and feature extraction, different machine learning techniques are applied to the database namely,
1)	Multinomial Naïve Bayes
2)	Support Vector Machine
3)	K Nearest Neighbors  

Data Preprocessing, Feature Vector and Models Used:  

1)	The Dataset had two columns: 1st containing the class of data ham or spam and 2nd containing a string which is the text message.

2)	All English Stopwords were imported from NLTK and were removed if found in the sentences.

3)	We used a basic Count vectorizer from Sklearn library in order to tokenize and vectorize the string of text. The Count Vectorizer provides a simple way to both tokenize a collection of text documents and build a vocabulary of known words, but also to encode new documents using that vocabulary.

It can be used as follows:

a)	Create an instance of the CountVectorizer class.

b)	Call the fit() function in order to learn a vocabulary from document.

c)	Call the transform() function on the document as needed to encode each as a vector.

An encoded vector is returned with a length of the entire vocabulary and an integer count for the number of times each word appeared in the document.

4)	 We got our numeric or real feature vector from string of text messages.

5)	 We next perform the test train split in the ratio of 70:30, we select the samples randomly.

6)	We feed the X_train, X_test, y_train, y_test to different ML models namely, Multinomial naïve bayes, Support vector machines, K nearest neighbours.

 
 Comparison of Outputs:   

Results obtained by our implemented models:

Unique values in the Class set:  ['ham' 'spam']

Number of ham messages in data set: 4825

Ham Count value 272

Number of spam messages in data set: 747

Spam Count value: 122

Training set has 3900 samples.
Testing set has 1672 samples.  

Multi-NB  
Accuracy in %:  
98.38516746411483  
F1 Score  
0.9382151029748284 
  
SVM  
Accuracy in %:  
98.20574162679426  
F1 Score  
0.9271844660194175 
  
KNN  
Accuracy in %:  
94.91626794258373  
F1 Score  
0.7632311977715878 


