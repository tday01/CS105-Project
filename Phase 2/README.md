# CS105-Project: Scraping, Cleaning, and EDA

###### jallybean_proj_phase2.ipynb

Program scrapes stockmonitor.com for top performing 100 Nasdaq stocks (live) and yahoo finance (historic).
All data is collected, cleaned, and saved to corresponding csv file.
Data includes symbol, name, price, volume, pChange, high, low.

Several visualizations are used to demonstrate the top 5 movers (live data) metrics as well as their
historic performance. I made these options easily configurable from the 'config' section
at the start of the jupyter notebook.

Each code portion is commented so that the reader can easily interpret each intended function.

## EDA

#### Visualization 1

Automatically finds best 5 movers from live data and shows past performance
(I did not use a histogram since occurence/frequency did not apply)

#### Visualization 2

Top 5 movers, sorted by percent change, best current mover is at bottom of graph

#### Visualization 3

Top 5 movers, historic volume

#### Visualization 4

Top 5 movers volume vs percent change

#### Visualization 5

All 100 stocks, percent change over historic

#### Visualization 6

All 100 stocks, parallel coordinates relationship: price -> volume -> high -> change -> low

#### Visualization 7

Top 5 boxplot, pChange

#### Visualization 8

All 100 stocks, 3D: pChang, Volume, Close

## Installation

Code is ready to run in jupyter notebook. 

'pip install' needed dependencies, or if using anaconda, 
install libraries through navigator/profile terminal.

## Usage

'Config' section is self-explanatory

run in jupyter notebook

