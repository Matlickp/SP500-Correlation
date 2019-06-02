# SP500-Data

## Why is correaltion important?

Correlation is the relationship between 2 or more things and, when it comes to investing, understanding the correlation of different stocks and asset classes plays a key part in diversification. 


## Objective:

The S&P500 is a stock index that tracks the 500 large companies by their market capitalization. This means evey company within it plays a role in the behavior of the index as a whole. Using daily adjusted closing prices of each of the 500 companies over a period of 4 years, we can create a correlation matrix so see how each companies stock behaves in relation to the others in the index. In practice you probably wouldn't create a matrix for 500 stocks but we could build upon the entire matrix with an app or zoom in on sections of it.

![S&P](Images/spbuilding.jpeg?raw=true "S&P")

## Data Gathering and Cleaning

All of the data was gathered using the pandas datareader with yahoo finance. Each ticker was given it's own .csv file of historical prices and then merged into one large .csv file and read into the main Jupyter Notebook using Pandas. The completed .csv of all the companies was then read into a dataframe and the correaltion calculation could be done. 

![Corr Table](Images/SP500CorrTable.jpg?raw=true "Corr Table")

## Visualizing

Using the dataframe of correlation coefficients we can then build a heatmap with annoted coefficients for added context and analysis.

![Matrix](Images/matrix.png?raw=true "Matrix")
