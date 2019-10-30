# Spam-Classifier

## Introduction
Recently unsolicited commercial / bulk e-mail also known as spam, become a big trouble over the internet. Spam is waste of time, storage space and communication bandwidth.

## Technologies Used
Machine learning field is a subfield from the broad field of artificial intelligence, this aims to make machines able to learn like human.

## Platform Used
SPYDER

## Project Description
The objective is to implement a Naïve Bayesian anti-spam filter to segregate spam from ham and measure its efficiency using various cost effective meeasures. 
A supervised learning approach is used to enable the filter to differentiate between spam and ham. The filter is trained on 70% off spam & ham corpus that requires Feature Extraction and calculation of spam probability of the extracted feature, fi , using a naïve 
Bayes.

## Training
1. Parse each email into its constituent tokens  
2. Generate a probability for each token W  
     S[W] = Cspam(W) / (Cham(W) + Cspam(W))  
3. Store spamminess values to a database  

## Testing 
We are testing the trained model on the testing set of the dataset.

## DETAILED ALGORITHM STEPS

### Step 1: Email pre-processing 
The content of email is received through our software, the information is extracted then as mentioned above, then the information (Feature) extracted is saved into a corresponding database. Every message was converted to a feature vector with 21700 attributes (this is approximately the number of different words in all the messages of the corpus). An attribute n was set to 1 if the corresponding word was present in a message and to 0 otherwise. This feature extraction scheme was used for all the algorithms.  

### Step 2: Description of the feature extracted 
Feature extraction module extract the spam text and the ham text, then produce feature dictionary and feature vectors as input of the selected algorithm, the function of feature extraction is to train and test the classifier [9]. For the train part, this module account frequency of words in the email text, we take words which the time of appearance is more than three times as the feature word of this class. And denote every email in training as a feature vector.  

### Step 3: Spam classification 
Through the steps above, we take standard classification email documents as training document, pretreatment of email, extract useful information, save into text documents according to fix format, split the whole document to words, extract the feature vector of spam document and translate into the form of vector of fix format. We look for the optimal classification using the selected algorithm which is constructed using the feature vector of spam documents.  

### Step 4: Performance evaluation 
In order to test the performance of above mentioned six methods, we used the most popular evaluation methods used by the spam filtering researchers. Spam Precision (SP), Spam Recall (SR), Accuracy (A). Spam Precision (SP) is the number of relevant documents identified as a  
 of Spam Correctly Classified  Nspam→spam 

## How to Run
1. Open Spyder or Jupyter Notebook 
2. Import the dataset from the directory where you saved the dataset
3. Run the whole program by entering ctrl+enter.
4. Observe the accracy.

## RESULTS 
After building the machine learning model we can predict that a email or messages on mobile phones etc.  is spam or ham (i.e Not  spam) by using this model. 
This model is trained on a huge dataset and has a accuracy of 98.7% for predicting a message is a  spam or not spam. 


 
