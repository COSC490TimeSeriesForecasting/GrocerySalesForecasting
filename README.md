# Grocery Sales Forecasting

The topic of our project is sales forecasting which falls in the realm of time-series forecasting. The main objective of this project is to predict the unit sales for a variety of products sold by Corporación Favorita, an Ecuadorian-based grocery retailer.  

Corporación Favorita is a large-scale grocery chain with hundreds of supermarkets spread across Ecuador and other South American countries. They sell over 200,000 products in their supermarkets. One of the biggest challenges for such large stores is the ability to make accurate predictions on the sales of different items so that they can stock up on their inventory accordingly. The emphasis is on the word “accurate” because if these predictions are overestimated than what is needed, then the grocers are stuck with a surplus of products (which, if perishable, could lead to enormous food wastages) and if the predictions are underestimated, then there is a shortage of products that leads to unhappy customers. The current forecasting methods are not usually automated and hence are not equipped to make such accurate predictions. Moreover, the prediction process becomes increasingly complex when factors like adding new retail stores and new products, the current market trends, and the ever-changing customer needs are taken into consideration.  

In this project, we aim to use robust machine learning algorithms to achieve precise predictions on the sales for the grocery store. These predictions would decrease the possibilities of food wastage and increase overall customer satisfaction.


## Objectives 

For the remainder of the term we will be focusing on the following: 

Initial data import, cleanup, and overview

Exploratory Data Analysis 

Identyfying optimal model based on gathered data and objective 

Model Development

Model evaluation and comparison



## Data 

The data from this project was obtained via a kaggle competition. The data is comprised of 7 datasets 
Url: https://www.kaggle.com/c/store-sales-time-series-forecasting/data

Train data - Sales, date ,store item , also contains information regarding whether the item was on sale and if it was on sale when it was sold. Data ranges from Jan 1, 2013 - Aug 15, 2017


Test data - The test data, having the same features as the training data. You will predict the target sales for the dates in this file.
The dates in the test data are for the 15 days after the last date in the training data.


Transactions - includes the number of transactions by store by day. 

Holidays_events -  contains a list of national holidays with a description

Stores -  a list of stores, with columns for location , type, and cluster. Type is not clearly identified and Cluster is a group of stores that has been pre-selected fue to similar charactersitics. There appears to be no in depth infomration of such characteristics. 


Oil - Daily oil prices. As ecuadors economy is dependent on oil this helps us explore the relationship between oil prices and grocery sales. It is important to note that the consumer is unaffected by these fluctuations as gas prices in Ecuador where subsidized throughout the time frame of this data. 

Items - A listing of each item sold in the stores (with an item number, not a name), the “family” (grocery, cleaning, bakery, and others), class (unclear what this means) and whether or not the item is perishable.


Additional Notes

Wages in the public sector are paid every two weeks on the 15 th and on the last day of the month. Supermarket sales could be affected by this.
A magnitude 7.8 earthquake struck Ecuador on April 16, 2016. People rallied in relief efforts donating water and other first need products which greatly affected supermarket sales for several weeks after the earthquake.

