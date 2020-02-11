## CS105-Project - Scraping and API

Scrapes from stockmonitor.com for Nasdaq 100 top performing stocks (intraday). 
The scraper finds price change, symbol, name, price, volume, high, low. Data is cleaned and
stored in a csv file.

The API code pulls the same category of data as the scraper, but stock performance is historical. 
Alpha Advnatage is the API used.

Merging these two datasets, we can compare historical and live stock performance for the top 100 
performing stocks on the nasdaq. 

## Installation

Scraper/API code is written in jupyter notebook. 

pip install needed dependencies, or if using anaconda, 
install libraries through navigator.

## Usage

Scraper - run in jupyter notebook

API code (Alpha Advantage) - run in jupyter notebook

## Upcoming Work

Use machine learning algorithm to suggest the best stock purchase on the Nasdaq-100 intraday. 
The model will train on historical data where the best performer of each day is known and then
the model will infer on live stock data.

