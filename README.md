# Edgar-AllanPoe
Using SEC's EDGAR to download quarterly financial statements and compare to historical stock movement of S&P 500 companies

## Code
* [Final Code used in Presentation](./Code/Edgar_AllanCode-Allyrs.ipynb)


## Resources Used
The base code used to find the Ticker and CIK values of all S&P 500 companies mines the data from the Wikipedia page on the S&P 500.
The base code can be found at: https://pythonprogramming.net/sp500-company-list-python-programming-for-finance/

The base code to querey Financial Statements from SEC's EDGAR was found thanks to Nick McCarthy.
The base code was found at: https://www.codeproject.com/Articles/1227765/Parsing-XBRL-with-Python

The Stock Data being used was accumulated and uploaded by Cam Nugent on kaggle.com.
The Stock Data runs through 02/08/2013 to 02/07/2018 and can be found at: https://www.kaggle.com/camnugent/sandp500/data

## Caveats
The Stock Data did not include Adjusted Close prices, so any evalutions could be effected by any Stock Splits or Dividends.
Different ContextRef ID formats are used between different companies and different years. Due to the time limitations on the project, I could not code it to dynamically find the CRef ID's, and instead I hard coded it to working with Microsoft's pre-2017 CRef ID Format.
