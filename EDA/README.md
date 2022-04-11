
# Overview

- 'eda.ipynb' and 'Data_Overview_Cleaning_EDA.ipynb' contain the inital EDA and exploration
- 'data_pipeline.ipynb merges the data and outputs a sample of the dataset. 
-  'EDA_Using_Final_Sample.ipynb' eda on unit sales after merging data.



# Data 

Train data:

The train data contained columns relating to product and sales for each day. For this dataset we had to deal with nan values  in the columns for products on promotion. We changed NaN values to 0 to signify these items were not on promotion. 


Transactions: 

The transactions dataset contains data regarding the amount of daily transactions in each store of the chain.  We had to deal with nan values and some outliers that would have affected the model.  They follow a clear seasonal pattern in which the number of transactions increases in the month of december due to the holidays and drops in the first days of the year.  The effect of the earthquake can also be observed 

Oil:
The oil dataset contained information regarding oil prices on different dates.  The main issue with this data set was the missing values in the oil prices for certain dates. In addition, oil prices for a lot of dates (that were present in the training set) were not provided. Therefore, for bringing in consistency between the dates in the train data and the oil data, we added the missing dates into the oil data set. The Nan values were filled by taking the average of the previous day’s and the next day’s oil price.  


Items:
The items data contained information regarding product class and family. From the EDA, we understood that the product family provided a broader categorization of products while the class variable was a more granular division within each family. So family provided a first level categorization of products and class provided a second level categorization. The items dataset also provides information whether the item is perishable or not. 

Stores:
The store data set specifies the city, state and the type for each favorita store. A few of the columns are ambiguous. For instance, we don’t know the basis on which the stores were classified into their types and clustered.As expected, the stores are located in Ecuador’s most populated cities-Quito and Guayaquil. 

Holidays:
The dataset contains information regarding important holidays and events that occurred in the time span captured by the training dataset. The dataset contains the type of the holiday, the location and region where the holiday or event is celebrated as well as whether the holiday is transferred to another day. The dataset included records of important events that occurred during that time span, for instance the 2014 Football Worldcup and the 2016 Earthquake that occurred in Ecuador. 
