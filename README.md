# RNN-LSTM-Foreseeing_the_Financial_Crisis

<p align="center">
  <img src="https://github.com/EXJUSTICE/RNN-LSTM-Foreseeing_the_Financial_Crisis/blob/master/RNNresults.png" >
  <em> Prediction results from model trained on pre-EDSC data (Jan 2006-Jan 2011), using moving average data over 20, 40, and 80 days.</em>
</p>

In this tutorial,we will be using the Kaggle “stock data” dataset to attempt to forecast stock prices. This dataset lists the performance of some of the major banks before, during, and after the financial crisis.

## Scenarios
To test the robustness of our system and better understand its limitations, we devised a series of scenarios where differing amounts of data was available for our model.

Scenario A: January 2006-December 2006 (pre-GFC data; 252 datapoints)


Scenario B: January 2006-January 2011 (post-GFC, pre-EDSC data;1260 datapoints)

## Procedure

* Import the dataset and create a dataframe of the closing price.
* Normalize our data to lie in between [0,1] using MinMaxScaler.
* Define the variables affecting length of predictions, in days.
* Create input data sequences (X and Y) of appropriate lengths, as defined in previous step.
* Split the data sequences into training, validation, and testing subsections.
* Build and train the model over 50 epochs.
* Plot our predictions against the actual historical data.

### Main tutorial

https://medium.com/gradientcrescent/foreseeing-armageddon-could-ai-have-predicted-the-financial-crisis-1a44ca62b4f5
