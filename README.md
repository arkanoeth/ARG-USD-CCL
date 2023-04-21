# ARG-USD-CCL

I wrote this code back in 2020 to help me calculate the CCL in Argentina. Basically, it's a way to figure out the implied exchange rate between local stocks and their ADRs. To do this, I used financial information from Invertir Online and created a formula that multiplies the local stock price by a certain number and divides it by the ADR price.

# Installation

The project requires the following dependencies:

requests

json

pandas

numpy

time

tabulate

matplotlib

To install the dependencies, use the package manager pip in the terminal:

*_pip install requests json pandas numpy time tabulate matplotlib_*

# Usage

To use the project, follow these steps:

1- Set up environment variables or a configuration file for the username and password.

2- Call the _execute_something()_ function.

The _execute_something()_ function fetches the stock quotes, calculates the CCL, creates a dataframe, displays the dataframe and plots the CCL.

# Functionality

Function to get access token

The _get_access_token(username, password)_ function takes in the **username** and **password** as parameters, sends a request to the API to get an access token and returns the access token and refresh token.

Function to fetch stock quotes

The _fetch_stock_quotes(symbols, mercado, bearer)_ function takes in the **symbols**, **mercado** and **bearer** as parameters, sends a request to the API to get the stock quotes and returns the last price of each stock.

Function to calculate CCL

The _calculate_ccl(local_quotes, adr_quotes, multiplier)_ function takes in the **local_quotes**, **adr_quotes** and **multiplier** as parameters, calculates the CCL and returns the CCL for each stock.

Main function
The _execute_something()_ function calls the _get_access_token()_, _fetch_stock_quotes()_ and _calculate_ccl()_ functions, creates a dataframe, displays the dataframe and plots the CCL.

# Possible future features

Additional analysis: Could be extended to provide additional analysis of the stock quotes, such as trend analysis, moving averages, or technical indicators.

More API options: Could be updated to use different APIs to fetch stock quotes, giving users more flexibility and options.

Interactive UI: Could be adapted to create an interactive user interface, where users could input their own symbols, market, and multiplier values, and see the results displayed in real-time.

Real-time updates: Could be updated to provide real-time updates of stock quotes and CCL calculations, allowing users to see the latest information as soon as it becomes available.

Alerting system: Could be updated to include an alerting system that notifies users when certain stock quotes or CCL values reach a certain threshold, allowing users to react quickly to market changes.

Machine learning integration: Could be adapted to incorporate machine learning algorithms to provide more accurate and predictive stock analysis.
