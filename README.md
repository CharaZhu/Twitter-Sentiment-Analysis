<p align="center">
  
  <h3 align="center"> Sentiment Analysis of 2019 Canadian Election Tweets </h3>
  <h5 align="center">Research question: What can public opinion on Twitter tell us about the Canadian political landscape in 2019?</h5>
  <h5 align="center">The purpose of this repo is to compute the sentiment of text information - tweets posted recently on Canadian Elections, 
get insight into the Canadian Elections and answer the Research question.</h5>
<h2 align="center">   </h2>
</p> 

  
#### TABLE OF CONTENTS 
- [Background](#background) 
- [Dataset](#dataset) 
- [Requirement](#requirement)
- Get Started
- [Technical Approach](#Technical Approach)
- [Limitations and Future Improvements](#Limitations and Future Improvements)
- [License](#license)
- [Reference](#Reference)  
<br/>


### Background
<h2 align="center"> </h2>

#### Sentiment Analysis  

A branch of Natural Language Processing (NLP) that allows us to determine algorithmically whether a statement or document is “positive” or “negative”. A technology of increasing importance in the modern society as it allows individuals and organizations to detect trends in public opinion by analyzing social media content. Keeping abreast of socio-political developments is especially important during periods of policy shifts such as election years, when both electoral candidates and companies can benefit from sentiment analysis by making appropriate changes to their campaigning and business strategies respectively.

### Dataset
<h2 align="center"> </h2>

- sentiment_analysis.csv: classified Twitter data containing a set of tweets which
have been analyzed and scored for their sentiment
- Candian_elections_2019.csv: Twitter data containing a set of tweets from 2019 on the Canadian elections, which needs to be analyzed for this assignment
 
### Requirement
<h2 align="center"> </h2>
Numpy, Scipy, Scikit, Matplotlib, Pandas, NLTK.
  
 
### Technical Approach
<h2 align="center"> </h2>
1. Data cleaning
 
Design a procedure that prepares the Twitter data for analysis by satisfying the requirements below.
o All html tags and attributes (i.e., /<[^>]+>/) are removed.
o Html character codes (i.e., &...;) are replaced with an ASCII equivalent.
o All URLs are removed.
o All characters in the text are in lowercase.
o All stop words are removed. Be clear in what you consider as a stop word.
o If a tweet is empty after pre-processing, it should be preserved as such.

2. Exploratory analysis  
o Design a simple procedure that determines the political party (Liberal, Conservatives
or New Democratic Party (NDC)) of a given tweet and apply this procedure to all the
tweets in the Canadian Elections dataset. A suggestion would be to look at relevant
words and hashtags in the tweets that identify to certain political parties or candidates.
What can you say about the distribution of the political affiliations of the tweets?
o Present a graphical figure (e.g. chart, graph, histogram, boxplot, word cloud, etc.) that
visualizes some aspect of the generic tweets in sentiment_analysis.csv and another
figure for the 2019 Canadian Elections tweets. All graphs and plots should be
readable and have all axes that are appropriately labelled.


3. Model preparation  
Split the generic tweets randomly into training data (70%) and test data (30%).
Prepare the data to try seven classification algorithms -- logistic regression, k-NN, Naive
Bayes, SVM, decision trees, Random Forest and XGBoost, where each tweet is
considered a single observation/example. In these models, the target variable is the
sentiment value, which is either positive or negative. Try two different types of features,
Bag of Words (word frequency) and TF-IDF on all 7

4. Model implementation and tuning  
Train models on the training data from generic tweets and apply the model to the
test data to obtain an accuracy value. Evaluate the same trained model with best
performance on the Canadian Elections data. How well do your predictions match the
sentiment labelled in the Canadian elections data?
Choose the model that has the best performance and visualize the sentiment
prediction results and the true sentiment for each of the 3 parties/candidates. Discuss
whether NLP analytics based on tweets is useful for political parties during election
campaigns.

Split the negative Canadian elections tweets into training data (70%) and test data
(30%). Use the true sentiment labels in the Canadian elections data instead of your

predictions from the previous part. Choose three algorithms from classification
algorithms (choose any 3 from logistic regression, k-NN, Naive Bayes, SVM, decision
trees, ensembles (RF, XGBoost)), train multi-class classification models to predict the
reason for the negative tweets. Tune the hyperparameters and chose the model with best
score to test your prediction reason for negative sentiment tweets. There are 5 different
negative reasons labelled in the dataset.
Feel free to combine similar reasons into fewer categories as long as you justify your
reasoning. You are free to define input features of your model using word frequency
analysis or other techniques.

5. Results  
Answer the research question stated above based on the outputs of your first model.
Describe the results of the analysis and discuss your interpretation of the results. Explain
how each party is viewed in the public eye based on the sentiment value. For the second
model, based on the model that worked best, provide a few reasons why your model may
fail to predict the correct negative reasons. Back up your reasoning with examples from
the test sets. For both models, suggest one way you can improve the accuracy of your
models.


#Limitations and Future Improvements)
● Try word embeddings (https://en.wikipedia.org/wiki/Word_embedding) and N-grams as feature
engineering techniques in addition to WF and TF-IDF.
● Explore Deep Learning algorithms and compare their performance to that of your best
performing classification model.
● Hyperparameter tuning for the models
● While the exploratory analysis section requires only two figures, you can explore the data
further. You can also display the results of the model visually.







### Built With

This section should list any major frameworks that you built your project using. Leave any add-ons/plugins for the acknowledgements section. Here are a few examples.
* [Bootstrap](https://getbootstrap.com)
* [JQuery](https://jquery.com)
* [Laravel](https://laravel.com)
 



<!-- GETTING STARTED -->
## Getting Started

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

### Prerequisites

This is an example of how to list things you need to use the software and how to install them.
* npm
  ```sh
  npm install npm@latest -g
  ```

### Installation

1. Get a free API Key at [https://example.com](https://example.com)
2. Clone the repo
   ```sh
   git clone https://github.com/your_username_/Project-Name.git
   ```
3. Install NPM packages
   ```sh
   npm install
   ```
4. Enter your API in `config.js`
   ```JS
   const API_KEY = 'ENTER YOUR API';
   ``` 
  
<!-- LICENSE -->
## License

[MIT](LICENSE) © Chara Zhu
