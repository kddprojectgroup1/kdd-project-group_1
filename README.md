KDD WeFive_HighFive (Group 1)
==


Team Members:

1. Akhil Chundarathil

2. Akhila Vemana

3. Akshara Gone

4. Keerthi Reddy Kandi

5. Koushik Koritala

Project Title: Mining and Modelling NYC Airbnb Data.
==



Project Objective: 
==


The project focuses on analysing the NYC Airbnb data and to predict the ratings of Airbnb based on guests experience, location, price range, nights of stay and other related features. 

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
* Rating ( 1-5 )

CRISP-DM Process:
==


1.Business/Research Understanding Phase : 
==


As Airbnb moves towards becoming an end-to-end travel platform, it is increasingly important for us to deliver travel insights that help people decide when to travel, where to go, and what to do on their trips. 

For example, 

* what are the most popular landmarks and neighborhoods in New York for a reasonable price?  
* Which Airbnb listings are best for families? 
* What are the type of reviews about an Airbnb? 

All of this content and context is helpful for vacation planners, and the more accurate, useful travel information we can provide, the more our users will trust us.

To scale our ability to answer these travel queries, we needed a systematic approach to storing and serving high-quality information about entities (e.g. ratings, cities, landmarks, events, etc.) and the relationships between them (e.g. the most popular landmark in a city for a reasonable price, the best neighbourhood to stay, etc.)

2.EDA and Data Preparation:
==

* Imputation techniques performed to handle missing values.
* A new "ratings" column is included for the hosts based on the neighbourhood group, price and days of availability of the airbnb.
* Based on the statistical information of the dataset the Outliers are removed. 
* Feature Scaling on some of the attributes are performed.
* Dropped some of the features which are not required for further phases.
* Next in Data Exploration, we get useful insights by visualizing different types of graphs plotted.

4.Machine Learning:
==

In the modelling phase, based on dataset we use and compare the models, select the best approproiate model for the datset.

* Classification: Naive Bayes(NB) to predict the probability of guests choosing the Airbnb given its location, price, ratings.
* Clustering: K-Nearest Neighbours(KNN) to know about which locations in NYC is popular for Airbnb's considering price, ratings.
* Regression: Linear regression(TF-IDF) to recommend Airbnb to guests by training and testing, based on their selection of features. 


5.Evaluation:
==

For the performance evaluation, based on the modelling done we use the metrics ROC curve, AUC value and Confusion matrix.

6.Conclusion:
==

Finally, we acheive useful insights from the model built based on pre-defined objectives.














