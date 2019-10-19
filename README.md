Team Name: WeFive_HighFive
==


Team Members:

1. Akhil Chundarathil

2. Akhila Vemana

3. Akshara Gone

4. Keerthi Reddy Kandi

5. Koushik Koritala

Project Title: Predictions and Analyzing New York City Airbnb Data.
==



Project Description: 
==


The project focuses on predicting and analyzing the ratings of customers, hosts of Airbnb's and summarizing useful insights of Airbnb's location of reasonable price based on features in the dataset.

Data and Source Description:
==


Dataset Link: https://www.kaggle.com/dgomonov/new-york-city-airbnb-open-data/kernels 

The metrics in the dataset for exploration, visualizations and predictions are:

* id-listing ID
* name- name of the listing
* host_id- host ID
* host_name- name of the host
* neighbourhood_group- location
* neighbourhood- area
* latitude- latitude coordinates
* longitude- longitude coordinates
* room_type- listing space type
* price- price in dollars
* minimum_nights- amount of nights minimum
* number_of_reviews- number of reviews
* last_review- latest review
* reviews_per_month- number of reviews per month
* calculated_host_listings_count- amount of listing per host16.
* availability_365- number of days when listing is available for booking

CRISP-DM Process:
==


1.Business/Research Understanding Phase : 
==


As Airbnb moves towards becoming an end-to-end travel platform, it is increasingly important for us to deliver travel insights that help people decide when to travel, where to go, and what to do on their trips. 

For example, 

* what are the most popular landmarks and neighborhoods in New York for a reasonable price?  
* Which Airbnb listings are best for families? 
* What is the most affordable time of year to visit New York?
* What are the type of reviews about an Airbnb and How are the ratings for a particular host of an Airbnb? 

All of this content and context is helpful for vacation planners, and the more accurate, useful travel information we can provide, the more our users will trust us.

To scale our ability to answer these travel queries, we needed a systematic approach to storing and serving high-quality information about entities (e.g. ratings, cities, landmarks, events, etc.) and the relationships between them (e.g. the most popular landmark in a city for a reasonable price, the best neighbourhood, etc.)

2.Data Understanding and EDA:
==

* After importing the dataset, we perform exploratory data analysis.
* First is to do data preprocessing. It has handling the missing data by imputation techniques, selecting the features for exploration and visualizations(In this dataset we are dropping some features which are not required for further steps).
* Included new "ratings" column for both customers and hosts based on the description of Airbnb and reviews by customers and using other features.
* Next in Data Exploration, we use the preprocessed data to get useful insights from visualizations and predictions.

3.Data Preparation:
==

Preparing the data for modelling in the further process. If needed planning to do the transformations on some of the features in the dataset.

4.Machine Learning:
==

In the modelling phase, planning to do the following modelling techniques and compare the models, select the best approproiate model for the datset.

* Classification: Naive Bayes(NB), Support Vector Machines(SVM)
* Clustering: K-Nearest Neighbours(KNN)
* Regression: Logistic regression
* Dividing the dataset into train and test data and further making fit and transform to the data

5.Evaluation:
==

For the Evaluation, we use some of the metrics like

* ROC curve
* AUC value
* Confusion matrix
* Accuracy, Precision and Recall

6.Conclusion:
==

Finally from the dataset we acheive useful insights based on pre-defined objectives.














