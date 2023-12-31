# RAPI Library / python

This is the official repository of the Reactioon API communication library for the python language.

## Focus

This library must meet some requirements, see the list below:

1. Simple and easy to use.
2. Easy to maintain/upgrade.
3. Reusable

## Usage

```python
import rapi

apikey={your-api-key}
secretkey={your-secret-key}

# method POST get price for get snapshot in exchange binance for currency usdt 

rapi.keys(apikey,secretkey)
r = rapi.request("POST","/api/v2/snapshots/cost",{'exchange':'binance','currency':'USDT'})
print(r.text)

# method GET get assets in your watchlist

rapi.keys(apikey,secretkey)
r =rapi.request("GET","/api/v2/watchlist/assets","")
print(r.text)
```

## Considerations
This library is under development and may change over time. The integrity of existing methods will be maintained to avoid compatibility issues in the future.

## Contributions
You can contribute to the development of the ecosystem by helping to improve this library. Feel free to improve and submit your work with a pull request.


@author Luis Pereira

