### KDD WeFive_HighFive (Group 1)


Team Members:

1. Akhil Chundarathil

2. Akhila Vemana

3. Akshara Gone

4. Keerthi Reddy Kandi

5. Koushik Koritala

# Project Title: Mining and Modeling NYC Airbnb Data.



### Project Objective: 


The project focuses on analyzing NYC Airbnb to predict the ratings of Airbnb based on their location, price range, guests experience (reviews) and other related features. 

### Data and Source Description:

Dataset Link: https://www.kaggle.com/dgomonov/new-york-city-airbnb-open-data/kernels 

The dataset has the following attributes :

* id
* name
* host_id
* host_name
* neighbourhood_group
* neighbourhood
* latitude
* longitude
* room_type
* price
* minimum_nights
* number_of_reviews
* last_review
* reviews_per_month
* calculated_host_listings_count
* availability_365
* RATINGS ( 1-5 : 1- Lowest, 5- Highest ).This column is not included in dataset, this target variable is added during the data preparation phase.

### CRISP-DM Process:


### 1.Business/Research Understanding Phase : 

**Domain Knowledge**: https://medium.com/airbnb-engineering/contextualizing-airbnb-by-building-knowledge-graph-b7077e268d5a

As Airbnb moves towards becoming an end-to-end travel platform, it is increasingly important for us to deliver travel insights that help people decide when to travel, where to go, and what to do on their trips. 

For example, 

* what are the most popular landmarks and neighborhoods in New York for a reasonable price?  
* Which Airbnb listings are best for families? 
* What are the type of reviews about an Airbnb? 


To scale our ability to answer these travel queries, we needed a systematic approach to storing and serving high-quality information about entities (e.g. ratings, cities, landmarks, events, etc.) and the relationships between them (e.g. the most popular landmark in a city for a reasonable price, the best neighbourhood to stay, etc.)

### 2.EDA and Data Preparation:


* A new "ratings" column is added based on the Airbnb location(neighborhood), price, reviews and days of availability.
(**Domain Knowledge** : https://www.airbnb.com/help/article/1257/how-do-star-ratings-work 

* Imputation techniques performed to handle missing values.
* Based on the statistical information of the dataset the Outliers are removed. 
* Feature Scaling on some of the attributes are performed.
* Dropped some of the features which are not required for further phases.
* Next in Data Exploration, we get useful insights by visualizing different types of graphs plotted (Insights are added as markdown in code).

### 3.Machine Learning:

For modeling, based on the dataset we use:

* Classification: Naive Bayes(NB) to predict the probability of guests choosing the Airbnb given its location, price, ratings.
* Association : We will use apriori algorithm for finding association rules between the attributes in our dataset. apriori class from apriori library will be used to find out the association rules between selected attributes like location,price and rating. min_lift parameter is used as a measure in the generating the association rules.
* Pipelining : We used pipeling for data preparation, feature extraction and modelling. Using normalization or standardization on the entire training dataset before learning would not be a valid test because the training dataset would have been influenced by the scale of the data in the test set. So we used pipelining to prevent this data leakage. We used FeatureUnion in pipeline which allows the results of multiple feature selection and extraction procedures to be combined into a larger dataset on which a model can be trained.
* Ensembling : By combining individual models, the ensemble model tends to be more flexible(less bias) and less data-sensitive (less variance). In our project, We are planning to use Random forest Algorithm as an ensemble model using bagging as the ensemble method and decision tree as the individual model.
* Bias : In the process of our analysis, we will use AIF360 method to mitigate bias. The approach we will use, called adversarial debiasing, is an example of a post-processing approach wherein bias is mitigated after the training takes place. 
* Regression: Linear regression(TF-IDF) to recommend Airbnb to guests by training and testing, considering the features chosen. 

### 4.Evaluation:

For the performance evaluation, based on the modeling is done we use the metrics ROC curve, AUC value, and Confusion matrix.

### 5.Conclusion:

Finally, we achieve useful insights from the model built based on pre-defined objectives. Our model will suggest guests in choosing suitable AirBnb for their trip in New York City considering their requirements( Budget, location, Ambience etc.. )














