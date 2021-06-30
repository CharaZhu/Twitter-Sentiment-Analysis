# Sentiment Analysis of 2019 Canadian Election Tweets  

##### The purpose of this repo is to compute the sentiment of tweets posted recently on Canadian Elections, get insight into the Canadian Elections and answer the Research question： What can public opinion on Twitter tell us about the Canadian political landscape in 2019?
</br>


#### TABLE OF CONTENTS 
- [Background](#background) 
- [Dataset](#dataset) 
- [Requirement](#requirement)
- [Technical Approach](#Technical-Approach)
- [Limitations and Future Improvements](#Limitations-and-Future-Improvements)
- [Reference](#Reference)  
<br/>

 
## Background
 
Sentiment Analysis is a branch of Natural Language Processing (NLP) that allows us to determine algorithmically whether a statement or document is “positive” or “negative”. It's a technology of increasing importance in the modern society as it allows individuals and organizations to detect trends in public opinion by analyzing social media content. Keeping abreast of socio-political developments is especially important during periods of policy shifts such as election years, when both electoral candidates and companies can benefit from sentiment analysis by making appropriate changes to their campaigning and business strategies respectively.
</br> </br> 


## Dataset
- sentiment_analysis.csv: classified Twitter data containing a set of tweets which
have been analyzed and scored for their sentiment
- Candian_elections_2019.csv: Twitter data containing a set of tweets from 2019 on the Canadian elections, which needs to be analyzed for this assignment
</br> </br>  
 
 
## Requirement
Numpy, Scipy, Scikit, Matplotlib, Pandas, NLTK.
</br> </br> 
 
 
## Technical-Approach

#### 1.Data cleaning: Design a procedure that prepares the Twitter data for analysis
- Remove all html tags and attributes (i.e., /<[^>]+>/)
- Replace Html character codes (i.e., &...;) with an ASCII equivalent
- Remove all URLs
- Remove all characters in the text are in lowercase
- Remove all stop words are removed
- Preserve empty tweet after pre-processing
</br> </br> 

#### 2. Exploratory analysis  
- Determine the political party of tweets in the Canadian Elections dataset.
- Visualization
</br> </br> 

#### 3. Model preparation 
- Classification algorithms: logistic regression, k-NN, Naive Bayes, SVM, decision trees, Random Forest and XGBoost
- Features: Bag of Words (word frequency),TF-IDF and N-grams
</br> </br> 
 
#### 4. Model implementation and tuning  
- Train classification model to predict the sentiment value (positive or negative) 
- Train multi-class classification models to predict the reason for the negative tweets. 
</br> </br> 
 

## Limitations and Future Improvements
* Try word embeddings (https://en.wikipedia.org/wiki/Word_embedding) as feature engineering techniques  
* Explore Deep Learning algorithms  

* Add more explanations (Requirement, algorithm) 
 

 
 
 
