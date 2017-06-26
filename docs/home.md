---
title: Home Page
permalink: home.html
---

# PyTradier (Work in Progress)

PyTradier is a library for interacting with the Tradier.com API for market data, company information, and trading actions through their brokerage. Since it is still early in development, the documentation for this python package will be updated as the project builds. 

### Getting Started
Every project must start by initiating in instance of the ```Tradier``` class:
```python
# create an instance of the tradier class and access the full API
trader = Tradier(token='aBcDeFg1234567', account_id='123456', sandbox=False)  
```
The parameters are as follows:
* ```token```: The API access token provided to you by Tradier. *Required.*
* ```account_id```: The account number associated with your Tradier brokerage account. Default is none, in case users only want the market data provided by Tradier, and not Tradier's brokerage system. *Optional.*
* ```sandbox```: Determines which endpoint of the API to use. Defaults to false, in which case the library will use the official API. If set to true, the library will use the developer's sandbox API. *Optional.*  