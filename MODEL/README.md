

# Model 

Given our knowledge of RNNs applied to time series forecasting, we chose to use an LSTM.  This decision was based on the fact that we want to deal with the problem of vanishing/exploding gradients. This will allow the model to make more educated predictions over longer time steps without losing context. Furthermore, a bidirectional layer was wrapped around it, as this will allow the model to learn the input sequence both forwards and backwards and embed this in the hidden states.  A snapshot of our code is provided in figure 2.1, while figure 2.2 shows the model in dot format.

# Hyperparameters 

For hyperparameter tuning we took a variety of approaches. We used trail and error, as well as referencing others' work, and we even used an automated hyper parameter tuner to achieve optimal results.  We concluded that we obtained the best results by using a 3 layer Sequential model. It contains a bidirectional LSTM layer with 256 neurons, a dropout layer , and a dense layer. For the optimizer we used Adam with a 0.01 as the learning rate. The model ran for 45 epochs and had a batch size of 64. We also used time steps of 3 hoping that the additional context will improve the performance of the predictive model. 


# Error Metrics 

We used mean squared error as our loss function. In order to evaluate the progress through every epoch we plotted the results and to compare the loss of train and test data.  Mean squared error heavily penalizes large outliers. This was useful to us as our data had outliers such as in the case of the earthquake in 2016 and some specific dates.

Additionally, once values were inverted to their original scales we generated graphs that depict how close the predictions fit the actual data.  Finally, we computed the Root mean squared error to obtain an interpretable idea of the precision of our model. We obtained an RMSE of 742 units



# sources 

https://kth.diva-portal.org/smash/get/diva2:1214307/FULLTEXT01.pdf

https://github.com/curiousily/Deep-Learning-For-Hackers/blob/master/12.time-series-demand_prediction.ipynb