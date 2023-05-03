# MA5851-A3-Capstone
A3 Capstone project Web Crawler and NLP 

A brief intro into the project, project deliverables and methods followed.

Data Harvesting using the web crawler
The crawler is built using the Selenium and Chrome webdriver.
The first part is to build and use the crawler to harvest the data from the restaurantji.com.
The harvested data is stored into CSV file to be further used in the data analysis.
 
Data loading and Wrangling Procedures.
The data is loaded into the environment, checked for any missing values.
The data is cleaned, removed for any URLs or unwanted noise in the data like determiners.
Rather than Named Entity Recognition (NER) words relating to Nouns, proper Nouns, Verbs and Adjectives are retained
The data is visualised with the NLTK Frequency methods and top occurring words with distribution plots.
The top occurring words are checked with WordClouds and the distribution.
The word’s distribution is checked with histograms and descriptive statistics is shown for the distribution.
 
Application of Machine Learning(ML) algorithms and Natural Laguane Processing NLP tasks
Topic Modelling
The topics in the reviews are key to understanding the customer thoughts on the restaurants.
The topic modelling is done with:
The initial model is done with stochastic model Latent Dirichlet Allocation (LDA)
Optimal model is retained through Cross-Validation of topics through the iterative approach.
The Number of topics is chosen on the optimal model which is used to build the current model.
The optimal model built is visualised with Python LDA Visualisation (pyLDAvis) and topics through WordCloud.
The second model is the dimensionality reduction method Non-negative Matrix Factorisation(NMF).
The optimal model and number of topics is selected through iterative cross-validation approach.
The optimal topic number is used to build the model and topics are visualised through WordCloud.
The model efficiency is checked through Perplexity and Coherence Score.
A review is taken from the real world data and is used to check the model prediction and topic number recognition in the model.
 
Sentiment Analysis and Classification Models
Another key aspect is to understand the sentiment of the customer and their views
A Neural Network based sentiment analyser (from Flair-package) is used to understand the polarity scores.
The Analyser is trained to differentiate th sentiments into *Positive and Negative classes.
The Classification algorithm based on the Ensemble methods like XGBOOST and Random Forest methods are used.
A Grid-search method is used to pick the best model and the best model is applied in prediction.
The classification reports are done for both Train and Test data to understand the evaluation metrics.
In the classification model XGBoost has a better performance than Random Forest.
A Negative and Positive review is used to assess the prediction and the topics they point to.
