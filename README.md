# GSV-Volatility

## Introduction
The **GSV.R** file associated with this project replicates the analysis of [Google search keywords that best predict energy price volatility](https://www.sciencedirect.com/science/article/pii/S0140988317302517).
The code can be easily used to predict/explain volatility of any price or time series using two-step GARCH and Google Search Volume for relevant keywords as an additional explanatory variable.

## How To Run
The code includes step-by-step explanation of the different analysis sections.
### Required Data
The **Prices.csv** file includes daily nominal and real prices of Brent crude oil, WTI crude oil, New York Harbor gasoline, Gulf Coast gasoline, New York Harbor heating oil and gatural gas from Jan 1990.

To run the analysis, you would need to download Google Search Volume data from [Google Trends](https://trends.google.com) *separately* for each keyword. 
These data should then be incorporated in a single CSV file such that the first column is the data and the rest are the GSV data of that date.
### Required packages
Required packages are mentioned in **GSV.R**.

## Other Prices/Time Series
The code can be used to predict the volatility of bonds, stock market, and any other data with time series nature. Stock price data can be obtained using packages such
as *Quantmod* or *BatchGetSymbols*. Modify the code to use these data as the price series instead.

## Future Updates
Upcoming updates of this project include:
- Pulling Google trends data and prices directly from the web.
- Graphics and visualization.
- In-sample out-of-sample analysis.