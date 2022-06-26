# Stats-Arbitrage
This repo presents an implementation of the basic stats arbitrage in cryptocurrency market

The code is highly reproducable - even beyond the cryptocurrency market. I made some remarks below on how you can run the strategy on your computer.

You will need to
1. have an api of asset (not necessarily cryptos) prices
2. convert this asset price into a pandas dataframe in form of df({'Price':[enter price series for asset A], 'Date':[enter the date]}) - the order can't be exchanged
3. set an alpha level for stats test, for co-integration and series normality tests - default is 0.05
4. replace get_price function in class: this function will return a tuple (current price for asset A, current price for asset B)
5. write trade function: see comments for the trade function


Note: can get a signal without writing the trade function - the program will produce a .txt file on selected assets. 


