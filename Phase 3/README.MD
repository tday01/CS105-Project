# CS105-Project: Machine Learning for Stock Prediction

###### jellybean_proj_CS105.ipynb

Program scrapes stockmonitor.com for top performing 100 Nasdaq stocks (live data) 
and then extracts those symbols to get corresponding historic data from Yahoo Finance.
All data is collected, cleaned, and saved to corresponding csv files.
Data includes symbol, name, price, volume, pChange, high, low.

Two machine learning algorithms are used to make predictions about the stock data: 
Linear Regression & Neural Network Regressor. By using two ML algos, we can see how
their predictions compare. When making a buying decision, it’s probably wise to have 
a second opinion.

Both ML algos train on the historic data for each stock with the label being percent change.
The pCHange target will help the ML algos learn how much each stock changes each day based 
on performance.

Once each ML algo has made its prediction for each stock, we take the 5 largest predicted
percent change movers. Then, we find the lowest value and add that to all best predictions 
each for their corresponding algorithm. We do this to make the graphs easier to understand 
when comparing which stocks are favored to move more than others.

Finally, the first two bar charts demonstrate the best 5 predicted stocks for each ML algo, and
the third, top 5 current movers live. We expect to see at least one stock that the ML algos agree 
on, and that stock should be in the top 5 movers of the day by bell close.

## Results

We see 3 charts in the jupyter notebook indicating the two ML algos predictions and the top 5 live stocks.
The ML algos agree on three stocks as best buys based on predicted positive movement: 'GILD','AMD','MSFT'.

Among the best movers of the day and the 3 agreed upon above: 'GILD'.

We can see that the two ML algos correctly agreed upon 'GILD'. 'AMD' and 'MSFT' were also
positive movers, but not in the top 5 that day.

Had you run this notebook at market open and decided to buy 'GILD' based on the predictions, your investment would have grown more than 8% by bell close.

## Installation

'pip install' needed dependencies, or if using anaconda, 
install libraries through navigator/profile terminal.

## Usage

'Config' section is mostly self-explanatory

The program is meant to be run at the beginning of the trading day, 'updateLive = True'.
If you already have the historic data you need then simply leave 'updateHistoric = False'.

The program can be run after trading hours to see how the predictions performed, 'updateLive = True'.

Run in jupyter lab

