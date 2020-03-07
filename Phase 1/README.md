# CS105-Project: Scraping and API

###### scraper.ipynb

Scrapes stockmonitor.com for top performing 100 Nasdaq stocks (intraday). 
The scraper finds price change, symbol, name, price, volume, high, low. Data is cleaned and
saved to a csv file.

###### API_yahoo.ipynb

The API is through YahooFinancials. The API code pulls the same category of data as the scraper 
(and much more) but stock performance data is historical based on predetermined date range. However, 
live data may also be accessed through the API if desired. Data is saved to a csv file.

Merging these two datasets, we can compare historical and live stock performance for the top 100 
performing stocks on the Nasdaq-100(ndx) index.

## Installation

Code is ready to run in jupyter notebook. 

'pip install' needed dependencies, or if using anaconda, 
install libraries through navigator/profile terminal.

###### scraper.ipynb

requests,
pandas,
bs4

###### API_yahoo.ipynb

yahoofinancials,
pandas,
json

## Usage

scraper.ipynb - run in jupyter notebook

API_yahoo.ipynb - run in jupyter notebook

## Upcoming Work

Use machine learning algorithm to infer the best stock purchase on the Nasdaq-100 intraday. 
The model will train on historical data where the best performer of each day is known, and then
the model will infer from live stock data the best stock buy of the day.

