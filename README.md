# [NLP]-Review-clasiification-using-LSTM

#Problem statement- Conventional optimization functions such as the grid search method and Bayesian optimization method take a lot of time to optimize the hyperparameters of the LSTM model. this is primarily because it takes a lot of time to perform the test of accuracy for each architecture and for each learning rate value for a given architecture. This Project presents a very simple but powerful technique to optimize the hyperparameters in a much shorter time.

#Description-

The approach of this method is to optimize the number of layers first without caring about learning rate in stage 1. in stage 2 we can optimize the model for optimal learning rate for the given number of layers which we selected during stage 1.

In this particular example we will try to optimize the LSTM model to predict The positive and negative reviews on a given data set. Here, we will utilize a dataset comprising 50,000 movie reviews from IMDB. Although Keras provides a pre-downloaded dataset that is similar, it is only half the size. However, Keras' version has already undergone a conversion process where the text in the dataset is represented by integer tokens. This conversion is a vital step in natural language processing, which will also be demonstrated in this tutorial. Therefore, we will download the original text data instead of using Keras' preprocessed version.
