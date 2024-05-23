# Comparing `tmp/openmargin-0.0.2.tar.gz` & `tmp/openmargin-0.0.3.tar.gz`

## Comparing `openmargin-0.0.2.tar` & `openmargin-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 openmargin-0.0.2/arrow-markets.png
--rw-r--r--   0        0        0    36803 2020-02-02 00:00:00.000000 openmargin-0.0.2/options_data.png
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 openmargin-0.0.2/requirements.txt
--rw-r--r--   0        0        0    11493 2020-02-02 00:00:00.000000 openmargin-0.0.2/src/openmargin/auxiliary.py
--rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 openmargin-0.0.2/src/openmargin/example.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 openmargin-0.0.2/src/openmargin/init.py
--rw-r--r--   0        0        0    13305 2020-02-02 00:00:00.000000 openmargin-0.0.2/src/openmargin/risk.py
--rw-r--r--   0        0        0    35128 2020-02-02 00:00:00.000000 openmargin-0.0.2/LICENSE
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 openmargin-0.0.2/README.md
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 openmargin-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    45402 2020-02-02 00:00:00.000000 openmargin-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 openmargin-0.0.3/arrow-markets.png
+-rw-r--r--   0        0        0    36803 2020-02-02 00:00:00.000000 openmargin-0.0.3/options_data.png
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 openmargin-0.0.3/requirements.txt
+-rw-r--r--   0        0        0    11540 2020-02-02 00:00:00.000000 openmargin-0.0.3/src/openmargin/auxiliary.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 openmargin-0.0.3/src/openmargin/example.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 openmargin-0.0.3/src/openmargin/init.py
+-rw-r--r--   0        0        0    13614 2020-02-02 00:00:00.000000 openmargin-0.0.3/src/openmargin/risk.py
+-rw-r--r--   0        0        0    35801 2020-02-02 00:00:00.000000 openmargin-0.0.3/LICENSE
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 openmargin-0.0.3/README.md
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 openmargin-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    45388 2020-02-02 00:00:00.000000 openmargin-0.0.3/PKG-INFO
```

### Comparing `openmargin-0.0.2/arrow-markets.png` & `openmargin-0.0.3/arrow-markets.png`

 * *Files identical despite different names*

### Comparing `openmargin-0.0.2/options_data.png` & `openmargin-0.0.3/options_data.png`

 * *Files identical despite different names*

### Comparing `openmargin-0.0.2/src/openmargin/auxiliary.py` & `openmargin-0.0.3/src/openmargin/auxiliary.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,289 +1,284 @@
-import numpy as np
-import pandas as pd
-import requests
-import datetime
-
-from enum import Enum
-from Historic_Crypto import HistoricalData
-from scipy.stats import norm
-
-################################################
-# Miscellaneous
-################################################
-days_per_year = 365
-hours_per_year = 24 * days_per_year
-seconds_per_year = hours_per_year * 60 * 60
-
-DERIBIT_API_URL = "https://deribit.com/api/v2/"
-
-def cumsum_list(lists):   
-    cum_list = []   
-    l = len(lists)   
-    cum_list = [sum(lists[0:x:1]) for x in range(0, l+1)]
-    return cum_list[1:]
-
-################################################
-# Symbols
-################################################
-class Ticker(str, Enum):
-    AVAX = 'AVAX'
-    ETH = 'ETH'
-    BTC = 'BTC'
-
-    def __str__(self):
-        return f"{self.value}"
-    
-    @staticmethod
-    def cast(ticker):
-        try:
-            return Ticker(ticker.upper())
-        except:
-            raise Exception(f"Unsupported ticker '{ticker}'")
-
-deribit_symbols = [Ticker.ETH, Ticker.BTC]
-binance_symbols = {Ticker.AVAX: "AVAXUSDT", Ticker.ETH: "ETHUSDT", Ticker.BTC: "BTCUSDT"}
-coingecko_ids = {Ticker.AVAX: "avalanche-2", Ticker.ETH: "ethereum", Ticker.BTC: "bitcoin"}
-historic_ids = {Ticker.AVAX: "AVAX-USD", Ticker.ETH: "ETH-USD", Ticker.BTC: "BTC-USD"}
-
-################################################
-# Spot & Option Data Retrieval
-################################################
-def get_underlier_price(ticker: str):
-    """
-        Get spot price of underlying asset from Binance (or CryptoWatch if rate limit is reached).
-
-        INPUTS:
-            ticker - Symbol of underlying asset.
-
-        OUTPUTS:
-            Spot price of specified underlying asset.
-    """
-
-    # Cast ticker to enum type
-    ticker = Ticker.cast(ticker)
-
-    # Using Binance API to get latest price
-    response = requests.get(
-        f"https://api.binance.com/api/v3/ticker/price?symbol={binance_symbols[ticker]}"
-    )
-    response_json = response.json()
-    # If Binance tells us we have been making too many requests, use Cryptowatch
-    if 'code' in response_json and response_json['code'] == -1003:
-        # Use CryptoWatch API to get latest price
-        response = requests.get(
-            f"https://api.cryptowat.ch/markets/binance/{binance_symbols[ticker]}/price"
-        )
-
-        try:
-            spot_price = float(response.json()['result']['price'])
-        except:
-            raise Exception("Could not retrieve underlying spot price from Cryptowatch.")
-    else:
-        try:
-            spot_price = float(response.json()['price'])
-        except:
-            raise Exception("Could not retrieve underlying spot price from Binance.")
-
-    return spot_price
-
-def get_historical_prices(ticker: Ticker, sampling_freq = 1, steps = 1e3):
-
-    steps = steps + 1
-    # sampling_freq = 1 # hours
-    sampling_freq_in_seconds = int(1 * 60 * 60)
-
-    hour_steps = steps * sampling_freq
-    end_date = datetime.datetime.today()
-    end_date.replace(minute=0, second=0, microsecond=0)
-    start_date = datetime.datetime.today() - datetime.timedelta(hours=hour_steps)
-    end_date = end_date.strftime("%Y-%m-%d-%H") + "-00"
-    start_date = start_date.strftime("%Y-%m-%d-%H") + "-00"
-
-    prices = pd.DataFrame()
-    prices = HistoricalData(historic_ids[ticker], sampling_freq_in_seconds, start_date, end_date, verbose = False).retrieve_data()
-
-    prices = prices['close'].to_numpy()
-    prices = prices[0::sampling_freq]
-
-    return prices
-
-def deribit_option_data(ticker, utcnow):
-    # Construct parameters for getting all instruments from Deribit's API
-    get_instruments_api_params = {
-        "currency": ticker,
-        "kind": "option",
-        "expired": "false"
-    }
-
-    try:
-        get_instruments_api_response = requests.get(DERIBIT_API_URL + '/public/get_instruments', get_instruments_api_params)
-        get_instruments_json = get_instruments_api_response.json()
-        instruments = get_instruments_json['result']
-    except:
-        raise Exception("There was an error collecting instrument data from Deribit")
-
-    num_fridays_to_look_ahead = 52 # Number of Fridays to look ahead to
-    seconds_per_week = 7 * 24 * 60 * 60
-    day_number = utcnow.weekday()
-    # Get date of next Friday (if it is a Friday, next weeks Friday)
-    if day_number >= 4:
-        first_friday = int((utcnow.replace(hour=8, minute=0, second=0, microsecond=0) + datetime.timedelta(days=-day_number, weeks=1) + datetime.timedelta(days=4)).timestamp())
-    elif day_number < 4:
-        first_friday = int((utcnow.replace(hour=8, minute=0, second=0, microsecond=0) - datetime.timedelta(days=day_number) + datetime.timedelta(days=4)).timestamp())
-
-    # Get expirations for num_fridays_to_look_ahead following the friday closest to today
-    months = ["JAN", "FEB", "MAR", "APR", "MAY", "JUN", "JUL", "AUG", "SEP", "OCT", "NOV", "DEC"]
-
-    expiration_strings = set()
-    for j in range(num_fridays_to_look_ahead):
-        ts = datetime.datetime.utcfromtimestamp(first_friday + j*seconds_per_week)
-        day = ts.day
-        month = months[ts.month-1]
-        year = f'{ts.year}'[2:]
-        hrexpiration = f'{day}{month}{year}'
-        expiration_strings.add(hrexpiration)
-
-    # Arrays for tracking quote data
-    log_moneynesses = []
-    expiration_datetimes = [] # Set of all expirations
-    yearly_times_to_expiration = [] # Set of all times to expiration
-    strikes = []
-    contract_types = []
-    spot_prices = []
-    yearly_mark_implied_volatilities = []
-    mark_prices = []
-    prices = []
-
-    # Loop through all instruments for the specified ticker
-    for instrument in instruments:
-        # Split instrument name into costituent parts
-        split_instrument_name = instrument['instrument_name'].split('-')
-        expiration_string = split_instrument_name[1] # Extract expiration string
-
-        # If expiration of current instrument is not one of the expirations we are looking for, continue to next instrument
-        if expiration_string not in expiration_strings: 
-            continue
-
-        # Construct order book parameters for API request
-        order_book_api_params = {
-            "instrument_name": instrument['instrument_name'],
-            "depth": 1 # Taken out of a hat
-        }
-
-        # Attempt to retrieve response from API request. Proceed to next instrument if there is an error
-        try:
-            order_book_api_response = requests.get(DERIBIT_API_URL + "/public/get_order_book", order_book_api_params)
-            order_book_json = order_book_api_response.json()
-        except Exception as e: # Check for API response exception
-            print(f"Error getting book data for instrument \"{instrument['instrument_name']}\": {e}")
-            continue # Proceed to next instrument if error with current one
-        
-        # Extract data into more readable variables
-        expiration_timestamp_millis = instrument['expiration_timestamp'] # Expiration in milliseconds
-        expiration_timestamp_seconds = expiration_timestamp_millis / 10**3
-        tte_in_millis = expiration_timestamp_millis - (utcnow.timestamp() * 10**3)
-        tte_in_seconds = tte_in_millis / 10**3
-        tte_in_years = tte_in_seconds / seconds_per_year
-        expiration = datetime.datetime.utcfromtimestamp(expiration_timestamp_seconds)
-        strike = float(split_instrument_name[2])
-        contract_type = split_instrument_name[-1] # Extract contract type string ("P" or "C")
-
-        # Get underlying price from deribit quote data and compute moneyness/log moneyness
-        spot_price = order_book_json['result']['underlying_price']
-        log_moneyness = np.log(strike / spot_price)
-
-        # Implied volatility from Deribit is yearly as percent (if yearly vol is 0.12, it comes back as 12)
-        yearly_mark_implied_volatility = order_book_json['result']['mark_iv'] / 100
-        
-        # Option Price denominated in Token & Usd
-        mark_price = order_book_json['result']['mark_price']
-        price = mark_price * spot_price
-
-        # Update arrays/sets to include relevant information
-        expiration_datetimes.append(expiration)
-        yearly_times_to_expiration.append(tte_in_years)
-        strikes.append(strike)
-        log_moneynesses.append(log_moneyness)
-        contract_types.append(contract_type)
-        spot_prices.append(spot_price)
-        yearly_mark_implied_volatilities.append(yearly_mark_implied_volatility)
-        mark_prices.append(mark_price)
-        prices.append(price)
-
-    # Cast all arrays to numpy arrays for computational conveniences
-    expiration_datetimes = np.array(expiration_datetimes)
-    yearly_times_to_expiration = np.array(yearly_times_to_expiration)
-    strikes = np.array(strikes)
-    log_moneynesses = np.array(log_moneynesses)
-    contract_types = np.array(contract_types)
-    spot_prices = np.array(spot_prices)
-    yearly_mark_implied_volatilities = np.array(yearly_mark_implied_volatilities)
-    mark_prices = np.array(mark_prices)
-    prices = np.array(prices)
-
-    return (
-        expiration_datetimes,
-        yearly_times_to_expiration,
-        strikes,
-        log_moneynesses,
-        contract_types,
-        spot_prices,
-        yearly_mark_implied_volatilities,
-        mark_prices,
-        prices
-    )
-
-################################################
-# Option Formulas
-################################################
-N = norm.cdf
-
-def bs_call(S, K, T, r, sigma):
-    d1 = (np.log(S/K) + (r + sigma**2/2)*T) / (sigma*np.sqrt(T))
-    d2 = d1 - sigma * np.sqrt(T)
-    return S * N(d1) - K * np.exp(-r*T)* N(d2)
-
-def bs_put(S, K, T, r, sigma):
-    d1 = (np.log(S/K) + (r + sigma**2/2)*T) / (sigma*np.sqrt(T))
-    d2 = d1 - sigma* np.sqrt(T)
-    return K*np.exp(-r*T)*N(-d2) - S*N(-d1)
-
-def binary_vol_finder(contract_type,option_price,spot_price,strike,T,r):
-
-    sigma_bounds = np.arange(0.01, 2, 0.0001)
-    """ Perform Binary Search """
-
-    left, right = 0, len(sigma_bounds) - 1
-    while left <= right:
-        # Get midpoint of indices
-        mid = (left + right) // 2 # double forward slash means integer division
-        _iv = sigma_bounds[mid]
-
-        # Compute the option price using sigma at the `mid` index
-        if contract_type == 'C':
-            _option_price = bs_call(spot_price, strike, T, r, _iv)
-        else: # Put
-            _option_price = bs_put(spot_price, strike, T, r, _iv)
-
-        # Check if the computed option price is within some threshold of the true option price
-        # If the computed option price is smaller, the sigma must be increased, so we move `left` above `mid`
-        # If the computed option price is larger, the sigma must be decreased, so we move `right` below `mid`
-        if abs(_option_price - option_price) < 1e-8:
-            return sigma_bounds[mid]
-        elif _option_price < option_price:
-            left = mid + 1
-        else:
-            right = mid - 1
-
-    # Compute the option price using sigma at the `mid` index
-    _iv = sigma_bounds[right]
-    if contract_type == 'C':
-        _option_price = bs_call(spot_price, strike, T, r, _iv)
-    else: # Put
-        _option_price = bs_put(spot_price, strike, T, r, _iv)
-
-    # If we are here, then we have searched the whole sigma space
-    # and nothing was within the threshold of the true option price.
-    # At this point, left > right. It is also possible that left == len(sigma_bounds)
-    # therefore we should return sigma_bounds[right] to avoid out of bounds errors.
-    return sigma_bounds[right]
+import numpy as np
+import pandas as pd
+import requests
+import datetime
+
+from enum import Enum
+from Historic_Crypto import HistoricalData
+from scipy.stats import norm
+
+################################################
+# Miscellaneous
+################################################
+days_per_year = 365
+hours_per_year = 24 * days_per_year
+seconds_per_year = hours_per_year * 60 * 60
+
+DERIBIT_API_URL = "https://deribit.com/api/v2/"
+
+def cumsum_list(lists):   
+    cum_list = []   
+    l = len(lists)   
+    cum_list = [sum(lists[0:x:1]) for x in range(0, l+1)]
+    return cum_list[1:]
+
+################################################
+# Symbols
+################################################
+class Ticker(str, Enum):
+    AVAX = 'AVAX'
+    ETH = 'ETH'
+    BTC = 'BTC'
+
+    def __str__(self):
+        return f"{self.value}"
+    
+    @staticmethod
+    def cast(ticker):
+        try:
+            return Ticker(ticker.upper())
+        except:
+            raise Exception(f"Unsupported ticker '{ticker}'")
+
+deribit_symbols = [Ticker.ETH, Ticker.BTC]
+binance_symbols = {Ticker.AVAX: "AVAXUSDT", Ticker.ETH: "ETHUSDT", Ticker.BTC: "BTCUSDT"}
+coingecko_ids = {Ticker.AVAX: "avalanche-2", Ticker.ETH: "ethereum", Ticker.BTC: "bitcoin"}
+historic_ids = {Ticker.AVAX: "AVAX-USD", Ticker.ETH: "ETH-USD", Ticker.BTC: "BTC-USD"}
+
+################################################
+# Spot & Option Data Retrieval
+################################################
+def get_underlier_price(ticker: str):
+    """
+        Get spot price of underlying asset from Binance (or CryptoWatch if rate limit is reached).
+
+        INPUTS:
+            ticker - Symbol of underlying asset.
+
+        OUTPUTS:
+            Spot price of specified underlying asset.
+    """
+
+    # Cast ticker to enum type
+    ticker = Ticker.cast(ticker)
+
+    # Using Binance API to get latest price
+    response = requests.get(
+        f"https://api.binance.com/api/v3/ticker/price?symbol={binance_symbols[ticker]}"
+    )
+    response_json = response.json()
+    # If Binance tells us we have been making too many requests, use Cryptowatch
+    if 'code' in response_json and response_json['code'] == 0:
+        # Use Binance.US
+        response = requests.get(
+            f"https://api.binance.com/api/v3/ticker/price?symbol={binance_symbols[ticker]}"
+        )
+
+    try:
+        spot_price = float(response.json()['price'])
+    except:
+        raise Exception("Could not retrieve underlying spot price from Binance.")
+
+    return spot_price
+
+def get_historical_prices(ticker: Ticker, sampling_freq = 1, steps = 1e3):
+
+    steps = steps + 1
+    # sampling_freq = 1 # hours
+    sampling_freq_in_seconds = int(1 * 60 * 60)
+
+    hour_steps = steps * sampling_freq
+    end_date = datetime.datetime.today()
+    end_date.replace(minute=0, second=0, microsecond=0)
+    start_date = datetime.datetime.today() - datetime.timedelta(hours=hour_steps)
+    end_date = end_date.strftime("%Y-%m-%d-%H") + "-00"
+    start_date = start_date.strftime("%Y-%m-%d-%H") + "-00"
+
+    prices = pd.DataFrame()
+    prices = HistoricalData(historic_ids[ticker], sampling_freq_in_seconds, start_date, end_date, verbose = False).retrieve_data()
+
+    prices = prices['close'].to_numpy()
+    prices = prices[0::sampling_freq]
+
+    return prices
+
+def deribit_option_data(ticker, utcnow):
+    # Construct parameters for getting all instruments from Deribit's API
+    get_instruments_api_params = {
+        "currency": ticker,
+        "kind": "option",
+        "expired": "false"
+    }
+
+    try:
+        get_instruments_api_response = requests.get(DERIBIT_API_URL + '/public/get_instruments', get_instruments_api_params)
+        get_instruments_json = get_instruments_api_response.json()
+        instruments = get_instruments_json['result']
+    except:
+        raise Exception("There was an error collecting instrument data from Deribit")
+
+    num_fridays_to_look_ahead = 52 # Number of Fridays to look ahead to
+    seconds_per_week = 7 * 24 * 60 * 60
+    day_number = utcnow.weekday()
+    # Get date of next Friday (if it is a Friday, next weeks Friday)
+    if day_number >= 4:
+        first_friday = int((utcnow.replace(hour=8, minute=0, second=0, microsecond=0) + datetime.timedelta(days=-day_number, weeks=1) + datetime.timedelta(days=4)).timestamp())
+    elif day_number < 4:
+        first_friday = int((utcnow.replace(hour=8, minute=0, second=0, microsecond=0) - datetime.timedelta(days=day_number) + datetime.timedelta(days=4)).timestamp())
+
+    # Get expirations for num_fridays_to_look_ahead following the friday closest to today
+    months = ["JAN", "FEB", "MAR", "APR", "MAY", "JUN", "JUL", "AUG", "SEP", "OCT", "NOV", "DEC"]
+
+    expiration_strings = set()
+    for j in range(num_fridays_to_look_ahead):
+        ts = datetime.datetime.utcfromtimestamp(first_friday + j*seconds_per_week)
+        day = ts.day
+        month = months[ts.month-1]
+        year = f'{ts.year}'[2:]
+        hrexpiration = f'{day}{month}{year}'
+        expiration_strings.add(hrexpiration)
+
+    # Arrays for tracking quote data
+    log_moneynesses = []
+    expiration_datetimes = [] # Set of all expirations
+    yearly_times_to_expiration = [] # Set of all times to expiration
+    strikes = []
+    contract_types = []
+    spot_prices = []
+    yearly_mark_implied_volatilities = []
+    mark_prices = []
+    prices = []
+
+    # Loop through all instruments for the specified ticker
+    for instrument in instruments:
+        # Split instrument name into costituent parts
+        split_instrument_name = instrument['instrument_name'].split('-')
+        expiration_string = split_instrument_name[1] # Extract expiration string
+
+        # If expiration of current instrument is not one of the expirations we are looking for, continue to next instrument
+        if expiration_string not in expiration_strings: 
+            continue
+
+        # Construct order book parameters for API request
+        order_book_api_params = {
+            "instrument_name": instrument['instrument_name'],
+            "depth": 1 # Taken out of a hat
+        }
+
+        # Attempt to retrieve response from API request. Proceed to next instrument if there is an error
+        try:
+            order_book_api_response = requests.get(DERIBIT_API_URL + "/public/get_order_book", order_book_api_params)
+            order_book_json = order_book_api_response.json()
+        except Exception as e: # Check for API response exception
+            print(f"Error getting book data for instrument \"{instrument['instrument_name']}\": {e}")
+            continue # Proceed to next instrument if error with current one
+        
+        # Extract data into more readable variables
+        expiration_timestamp_millis = instrument['expiration_timestamp'] # Expiration in milliseconds
+        expiration_timestamp_seconds = expiration_timestamp_millis / 10**3
+        tte_in_millis = expiration_timestamp_millis - (utcnow.timestamp() * 10**3)
+        tte_in_seconds = tte_in_millis / 10**3
+        tte_in_years = tte_in_seconds / seconds_per_year
+        expiration = datetime.datetime.utcfromtimestamp(expiration_timestamp_seconds)
+        strike = float(split_instrument_name[2])
+        contract_type = split_instrument_name[-1] # Extract contract type string ("P" or "C")
+
+        # Get underlying price from deribit quote data and compute moneyness/log moneyness
+        spot_price = order_book_json['result']['underlying_price']
+        log_moneyness = np.log(strike / spot_price)
+
+        # Implied volatility from Deribit is yearly as percent (if yearly vol is 0.12, it comes back as 12)
+        yearly_mark_implied_volatility = order_book_json['result']['mark_iv'] / 100
+        
+        # Option Price denominated in Token & Usd
+        mark_price = order_book_json['result']['mark_price']
+        price = mark_price * spot_price
+
+        # Update arrays/sets to include relevant information
+        expiration_datetimes.append(expiration)
+        yearly_times_to_expiration.append(tte_in_years)
+        strikes.append(strike)
+        log_moneynesses.append(log_moneyness)
+        contract_types.append(contract_type)
+        spot_prices.append(spot_price)
+        yearly_mark_implied_volatilities.append(yearly_mark_implied_volatility)
+        mark_prices.append(mark_price)
+        prices.append(price)
+
+    # Cast all arrays to numpy arrays for computational conveniences
+    expiration_datetimes = np.array(expiration_datetimes)
+    yearly_times_to_expiration = np.array(yearly_times_to_expiration)
+    strikes = np.array(strikes)
+    log_moneynesses = np.array(log_moneynesses)
+    contract_types = np.array(contract_types)
+    spot_prices = np.array(spot_prices)
+    yearly_mark_implied_volatilities = np.array(yearly_mark_implied_volatilities)
+    mark_prices = np.array(mark_prices)
+    prices = np.array(prices)
+
+    return (
+        expiration_datetimes,
+        yearly_times_to_expiration,
+        strikes,
+        log_moneynesses,
+        contract_types,
+        spot_prices,
+        yearly_mark_implied_volatilities,
+        mark_prices,
+        prices
+    )
+
+################################################
+# Option Formulas
+################################################
+N = norm.cdf
+
+def bs_call(S, K, T, r, sigma):
+    d1 = (np.log(S/K) + (r + sigma**2/2)*T) / (sigma*np.sqrt(T))
+    d2 = d1 - sigma * np.sqrt(T)
+    return S * N(d1) - K * np.exp(-r*T)* N(d2)
+
+def bs_put(S, K, T, r, sigma):
+    d1 = (np.log(S/K) + (r + sigma**2/2)*T) / (sigma*np.sqrt(T))
+    d2 = d1 - sigma* np.sqrt(T)
+    return K*np.exp(-r*T)*N(-d2) - S*N(-d1)
+
+def binary_vol_finder(contract_type,option_price,spot_price,strike,T,r):
+
+    sigma_bounds = np.arange(0.01, 2, 0.0001)
+    """ Perform Binary Search """
+
+    left, right = 0, len(sigma_bounds) - 1
+    while left <= right:
+        # Get midpoint of indices
+        mid = (left + right) // 2 # double forward slash means integer division
+        _iv = sigma_bounds[mid]
+
+        # Compute the option price using sigma at the `mid` index
+        if contract_type == 'C':
+            _option_price = bs_call(spot_price, strike, T, r, _iv)
+        else: # Put
+            _option_price = bs_put(spot_price, strike, T, r, _iv)
+
+        # Check if the computed option price is within some threshold of the true option price
+        # If the computed option price is smaller, the sigma must be increased, so we move `left` above `mid`
+        # If the computed option price is larger, the sigma must be decreased, so we move `right` below `mid`
+        if abs(_option_price - option_price) < 1e-8:
+            return sigma_bounds[mid]
+        elif _option_price < option_price:
+            left = mid + 1
+        else:
+            right = mid - 1
+
+    # Compute the option price using sigma at the `mid` index
+    _iv = sigma_bounds[right]
+    if contract_type == 'C':
+        _option_price = bs_call(spot_price, strike, T, r, _iv)
+    else: # Put
+        _option_price = bs_put(spot_price, strike, T, r, _iv)
+
+    # If we are here, then we have searched the whole sigma space
+    # and nothing was within the threshold of the true option price.
+    # At this point, left > right. It is also possible that left == len(sigma_bounds)
+    # therefore we should return sigma_bounds[right] to avoid out of bounds errors.
+    return sigma_bounds[right]
```

### Comparing `openmargin-0.0.2/src/openmargin/example.py` & `openmargin-0.0.3/src/openmargin/example.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-import random
-import datetime
-import pandas as pd
-
-from openmargin.risk import RiskConfig, PricePathGenerator, VAR, RiskModel, RiskCalc
-from openmargin.auxiliary import get_underlier_price, deribit_option_data
-
-################################################################
-# Locked Margin Calculator
-################################################################
-ticker = "eth"
-
-expiration = datetime.datetime.strptime('2024-09-27 08:00:00', "%Y-%m-%d %H:%M:%S")
-strike = 7000.0
-kind = "C"
-position = -1
-portfolio = {'expiration': expiration, 'strike': strike, 'kind': kind, 'position': position}
-portfolio = pd.DataFrame([portfolio],columns = ["expiration", "strike", "kind", "position"])
-
-risk_calculator = RiskCalc(ticker = ticker, portfolio = portfolio)
-print(risk_calculator.get_margin())
-
-#? Custom Inputs
-################################################################
-# Risk Parameters
-################################################################
-r = 0.05
-sampling_frequency = 1 # hours
-steps = 24
-
-risk_params = RiskConfig(r, sampling_frequency, steps)
-
-################################################################
-# Price Paths
-################################################################
-ticker = "eth"
-spot = get_underlier_price(ticker)
-number_of_paths = 1_000
-
-price_paths = PricePathGenerator(ticker = ticker, risk_params = risk_params, spot = spot, number_of_paths = number_of_paths)
-
-sample_paths = price_paths.generate_paths()
-
-################################################################
-# Options Data
-################################################################
-utcnow = datetime.datetime.now(tz=datetime.timezone.utc)
-(expiration_datetimes, yearly_times_to_expiration, strikes, log_moneynesses, contract_types, spot_prices, yearly_mark_implied_volatilities, mark_prices, prices) = deribit_option_data(ticker, utcnow)
-options_data = pd.DataFrame([spot_prices, expiration_datetimes, yearly_times_to_expiration, strikes, log_moneynesses, contract_types, yearly_mark_implied_volatilities, mark_prices, prices]).T
-options_data.columns = ['spot', 'expiration','tte','strike', 'log_money', 'kind','mark_iv','mark_price', 'price']
-options_data = options_data.reset_index(drop=True)
-
-options_data.to_csv(f'risk/options_data.csv', index = False)
-# options_data = pd.read_csv(f'risk/options_data.csv', parse_dates=['expiration'])
-
-################################################################
-# Portfolio
-################################################################
-number_of_instruments = 1
-quantities = random.choices([-1, 1], k = number_of_instruments)
-portfolio = options_data.sample(n = number_of_instruments)
-portfolio['position'] = quantities
-portfolio = portfolio.drop(columns=['spot', 'tte', 'log_money', 'mark_iv', 'mark_price', 'price']).reset_index(drop=True)
-
-################################################################
-# Risk Model
-################################################################
-var_type = 'CVAR'
-var_threshold = 0.01
-margin_method = VAR(var_type, var_threshold)
-
-risk_model = RiskModel(margin_method)
-
-################################################################
-# Margin Calculator
-################################################################
-risk_calculator = RiskCalc(ticker, portfolio, options_data, risk_params, risk_model, price_paths)
-print(risk_calculator.get_margin())
+import random
+import datetime
+import pandas as pd
+
+from openmargin.risk import RiskConfig, PricePathGenerator, VAR, RiskModel, RiskCalc
+from openmargin.auxiliary import get_underlier_price, deribit_option_data
+
+################################################################
+# Locked Margin Calculator
+################################################################
+ticker = "eth"
+
+expiration = datetime.datetime.strptime('2024-09-27 08:00:00', "%Y-%m-%d %H:%M:%S")
+strike = 7000.0
+kind = "C"
+position = -1
+portfolio = {'expiration': expiration, 'strike': strike, 'kind': kind, 'position': position}
+portfolio = pd.DataFrame([portfolio],columns = ["expiration", "strike", "kind", "position"])
+
+risk_calculator = RiskCalc(ticker = ticker, portfolio = portfolio)
+print(risk_calculator.get_margin())
+
+#? Custom Inputs
+################################################################
+# Risk Parameters
+################################################################
+r = 0.05
+sampling_frequency = 1 # hours
+steps = 24
+
+risk_params = RiskConfig(r, sampling_frequency, steps)
+
+################################################################
+# Price Paths
+################################################################
+ticker = "eth"
+spot = get_underlier_price(ticker)
+number_of_paths = 1_000
+
+price_paths = PricePathGenerator(ticker = ticker, risk_params = risk_params, spot = spot, number_of_paths = number_of_paths)
+
+sample_paths = price_paths.generate_paths()
+
+################################################################
+# Options Data
+################################################################
+utcnow = datetime.datetime.now(tz=datetime.timezone.utc)
+(expiration_datetimes, yearly_times_to_expiration, strikes, log_moneynesses, contract_types, spot_prices, yearly_mark_implied_volatilities, mark_prices, prices) = deribit_option_data(ticker, utcnow)
+options_data = pd.DataFrame([spot_prices, expiration_datetimes, yearly_times_to_expiration, strikes, log_moneynesses, contract_types, yearly_mark_implied_volatilities, mark_prices, prices]).T
+options_data.columns = ['spot', 'expiration','tte','strike', 'log_money', 'kind','mark_iv','mark_price', 'price']
+options_data = options_data.reset_index(drop=True)
+
+options_data.to_csv(f'risk/options_data.csv', index = False)
+# options_data = pd.read_csv(f'risk/options_data.csv', parse_dates=['expiration'])
+
+################################################################
+# Portfolio
+################################################################
+number_of_instruments = 1
+quantities = random.choices([-1, 1], k = number_of_instruments)
+portfolio = options_data.sample(n = number_of_instruments)
+portfolio['position'] = quantities
+portfolio = portfolio.drop(columns=['spot', 'tte', 'log_money', 'mark_iv', 'mark_price', 'price']).reset_index(drop=True)
+
+################################################################
+# Risk Model
+################################################################
+var_type = 'CVAR'
+var_threshold = 0.01
+margin_method = VAR(var_type, var_threshold)
+
+risk_model = RiskModel(margin_method)
+
+################################################################
+# Margin Calculator
+################################################################
+risk_calculator = RiskCalc(ticker, portfolio, options_data, risk_params, risk_model, price_paths)
+print(risk_calculator.get_margin())
```

### Comparing `openmargin-0.0.2/LICENSE` & `openmargin-0.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
+GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
 <https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `openmargin-0.0.2/README.md` & `openmargin-0.0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,123 +1,121 @@
-<p align="center"><img width=20% src="https://github.com/Arrow-Markets-Research/openmargin/raw/main/arrow-markets.png"></p>
-
-![Python](https://img.shields.io/badge/python-v3.8+-green.svg)
-![Version](https://img.shields.io/badge/version-0.0.1-red.svg)
-![License](https://img.shields.io/badge/license-GNU-blue.svg)
-
-# Open Margin
-
-Arrow Markets open source repository to calculate margin requirements for risky asset portfolios including crypto options portfolios.
-
-## Overview
-
-This repository includes a simplified version of the proprietary Arrow Markets margin calculator. <br />
-It uses VAR/CVAR methodology to compute the necessary margin required for a portfolio of BTC or ETH options. <br />
-Negative values refer to the cash margin needed for a given portfolio, while positive margin values count as credits. <br />
-For further details, please refer to the white paper ["Automated Margin Systems in Practice"](https://drive.google.com/file/d/12iX75pEvrZvwky-O8z6F1PeO65duMdyJ/view?usp=drive_link)
-
-## Installation
-
-```bash
-pip install openmargin
-```
-
-## Dependencies
-
-```bash
-pip install -r requirements.txt
-```
-## Usage
-
-Open Margin calculates the risk of an options portfolio through RiskCalc. <br />
-Once a compatible ticker and an options portfolio are provided portfolio margin can be computed with default parameters via: <br />
-
-```python
-import datetime
-import pandas as pd
-from openmargin.risk import RiskCalc
-
-ticker = "eth"
-
-expiration = datetime.datetime.strptime('2024-09-27 08:00:00', "%Y-%m-%d %H:%M:%S")
-strike = 7000.0
-kind = "C"
-position = -1
-portfolio = {'expiration': expiration, 'strike': strike, 'kind': kind, 'position': position}
-portfolio = pd.DataFrame([portfolio],columns = ["expiration", "strike", "kind", "position"])
-
-risk_calculator = RiskCalc(ticker, portfolio)
-risk_calculator.get_margin()
-
-```
-
-RiskCalc has four pillars that can be modified to generate the required margin.
-
-### Options Data
-Open Margin uses the current options data for BTC and ETH from Deribit. <br />
-To provide a different dataset, please provide a pandas dataframe containing options data similar to the one shown below: 
-
-<p align="left"><img src="https://github.com/Arrow-Markets-Research/openmargin/raw/main/options_data.png"></p>
-
-```python
-risk_calculator = RiskCalc(ticker, portfolio, options_data)
-risk_calculator.get_margin()
-```
-
-### Risk Configuration
-Three main risk factors are configured under RiskConfig. <br />
-Interest rate, sampling frequency and steps are the key parameters currently allowed for user customization. <br />
-Sampling frequency multiplied by steps determine the trading horizon that will be used to calculate margin values.
-
-```python
-from openmargin.risk import RiskConfig, RiskCalc
-
-r = 0.02
-sampling_frequency = 4 # hours
-steps = 6
-risk_params = RiskConfig(r, sampling_frequency, steps)
-
-risk_calculator = RiskCalc(ticker, portfolio, risk_params = risk_params)
-risk_calculator.get_margin()
-```
-
-### Risk Model
-RiskModel class determines the margin method used.
-Open Margin only allows VAR type margin methods in this public version.
-To select between VAR and CVAR and to change margin threshold:
-
-```python
-from openmargin.risk import VAR, RiskModel, RiskCalc
-
-var_type = 'VAR'
-var_threshold = 0.05
-margin_method = VAR(var_type, var_threshold)
-risk_model = RiskModel(margin_method)
-
-risk_calculator = RiskCalc(ticker, portfolio, risk_model = risk_model)
-risk_calculator.get_margin()
-```
-
-### Price Paths
-Path dependant methods like VAR/CVAR depend on future price paths. <br />
-1,000 paths are generated by default by PricePathGenerator. <br />
-Changes to the default number of paths can be made via:
-
-```python
-from openmargin.auxiliary import get_underlier_price
-from openmargin.risk import PricePathGenerator, RiskCalc
-
-spot = get_underlier_price(ticker)
-number_of_paths = 10_000
-price_paths = PricePathGenerator(ticker, risk_params, spot, number_of_paths)
-
-risk_calculator = RiskCalc(ticker, portfolio, price_paths = price_paths)
-risk_calculator.get_margin()
-```
-
-The paths can be generated with:
-
-```python
-sample_paths = price_paths.generate_paths()
-```
-
-Further customization examples can be found under example.py.
+<p align="center"><img width=20% src="https://github.com/Arrow-Markets-Research/openmargin/raw/main/arrow-markets.png"></p>
+
+![Python](https://img.shields.io/badge/python-v3.8+-green.svg)
+![Version](https://img.shields.io/badge/version-0.0.3-red.svg)
+![License](https://img.shields.io/badge/license-GNU-blue.svg)
+
+# Open Margin
+
+Arrow Markets open source repository to calculate margin requirements for risky asset portfolios including crypto options portfolios.
+
+## Overview
+
+This repository includes a simplified version of the proprietary Arrow Markets margin calculator. It uses VAR/CVAR methodology to compute the necessary margin required for a portfolio of BTC or ETH options. <br />
+Negative values refer to the cash margin needed for a given portfolio, while positive margin values count as credits. For further details, please refer to the white paper ["Automated Margin Systems in Practice"](https://drive.google.com/file/d/1y_113sCg4kOkU8lRDnyRjCovNpDMLNcM/view?usp=drive_link)
+
+## Installation
+
+```bash
+pip install openmargin
+```
+
+## Dependencies
+
+```bash
+pip install -r requirements.txt
+```
+## Usage
+
+Open Margin calculates the risk of an options portfolio through RiskCalc. <br />
+Once a compatible ticker and an options portfolio are provided portfolio margin can be computed with default parameters via: <br />
+
+```python
+import datetime
+import pandas as pd
+from openmargin.risk import RiskCalc
+
+ticker = "eth"
+
+expiration = datetime.datetime.strptime('2024-09-27 08:00:00', "%Y-%m-%d %H:%M:%S")
+strike = 7000.0
+kind = "C"
+position = -1
+portfolio = {'expiration': expiration, 'strike': strike, 'kind': kind, 'position': position}
+portfolio = pd.DataFrame([portfolio],columns = ["expiration", "strike", "kind", "position"])
+
+risk_calculator = RiskCalc(ticker, portfolio)
+risk_calculator.get_margin()
+
+```
+
+RiskCalc has four pillars that can be modified to generate the required margin.
+
+### Options Data
+Open Margin uses the current options data for BTC and ETH from Deribit. <br />
+To provide a different dataset, please provide a pandas dataframe containing options data similar to the one shown below: 
+
+<p align="left"><img src="https://github.com/Arrow-Markets-Research/openmargin/raw/main/options_data.png"></p>
+
+```python
+risk_calculator = RiskCalc(ticker, portfolio, options_data)
+risk_calculator.get_margin()
+```
+
+### Risk Configuration
+Three main risk factors are configured under RiskConfig. <br />
+Interest rate, sampling frequency and steps are the key parameters currently allowed for user customization. <br />
+Sampling frequency multiplied by steps determine the trading horizon that will be used to calculate margin values.
+
+```python
+from openmargin.risk import RiskConfig, RiskCalc
+
+r = 0.02
+sampling_frequency = 4 # hours
+steps = 6
+risk_params = RiskConfig(r, sampling_frequency, steps)
+
+risk_calculator = RiskCalc(ticker, portfolio, risk_params = risk_params)
+risk_calculator.get_margin()
+```
+
+### Risk Model
+RiskModel class determines the margin method used.
+Open Margin only allows VAR type margin methods in this public version.
+To select between VAR and CVAR and to change margin threshold:
+
+```python
+from openmargin.risk import VAR, RiskModel, RiskCalc
+
+var_type = 'VAR'
+var_threshold = 0.05
+margin_method = VAR(var_type, var_threshold)
+risk_model = RiskModel(margin_method)
+
+risk_calculator = RiskCalc(ticker, portfolio, risk_model = risk_model)
+risk_calculator.get_margin()
+```
+
+### Price Paths
+Path dependant methods like VAR/CVAR depend on future price paths. <br />
+1,000 paths are generated by default by PricePathGenerator. <br />
+Changes to the default number of paths can be made via:
+
+```python
+from openmargin.auxiliary import get_underlier_price
+from openmargin.risk import PricePathGenerator, RiskCalc
+
+spot = get_underlier_price(ticker)
+number_of_paths = 10_000
+price_paths = PricePathGenerator(ticker, risk_params, spot, number_of_paths)
+
+risk_calculator = RiskCalc(ticker, portfolio, price_paths = price_paths)
+risk_calculator.get_margin()
+```
+
+The paths can be generated with:
+
+```python
+sample_paths = price_paths.generate_paths()
+```
+
+Further customization examples can be found under example.py.
```

### Comparing `openmargin-0.0.2/pyproject.toml` & `openmargin-0.0.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[tool.hatch.build.targets.wheel]
-packages = ["src/openmargin"]
-
-[project]
-name = "openmargin"
-version = "0.0.2"
-authors = [
-  { name="Arrow Markets Research", email="ata@subharmonic.tech"},
-]
-description = "Arrow Markets repository for calculation margin requirements for crypto option portfolios."
-readme = "README.md"
-license = {file = 'LICENSE'}
-requires-python = ">=3.8"
-dependencies = [
-  "numpy>=1.23",
-  "pandas==1.5.3",
-  "scipy>=1.10",
-  "Requests>=2.31",
-  "Historic_Crypto>=0.1"]
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-    "Operating System :: OS Independent"
-]
-
-[project.urls]
-Homepage = "https://github.com/Arrow-Markets-Research/openmargin"
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[tool.hatch.build.targets.wheel]
+packages = ["src/openmargin"]
+
+[project]
+name = "openmargin"
+version = "0.0.3"
+authors = [
+  { name="Arrow Markets Research", email="ata@subharmonic.tech"},
+]
+description = "Arrow Markets repository for calculation margin requirements for crypto option portfolios."
+readme = "README.md"
+license = {file = 'LICENSE'}
+requires-python = ">=3.8"
+dependencies = [
+  "numpy>=1.23",
+  "pandas==1.5.3",
+  "scipy>=1.10",
+  "Requests>=2.31",
+  "Historic_Crypto>=0.1"]
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+    "Operating System :: OS Independent"
+]
+
+[project.urls]
+Homepage = "https://github.com/Arrow-Markets-Research/openmargin"
```

### Comparing `openmargin-0.0.2/PKG-INFO` & `openmargin-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: openmargin
-Version: 0.0.2
+Version: 0.0.3
 Summary: Arrow Markets repository for calculation margin requirements for crypto option portfolios.
 Project-URL: Homepage, https://github.com/Arrow-Markets-Research/openmargin
 Author-email: Arrow Markets Research <ata@subharmonic.tech>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -689,27 +689,25 @@
 Requires-Dist: requests>=2.31
 Requires-Dist: scipy>=1.10
 Description-Content-Type: text/markdown
 
 <p align="center"><img width=20% src="https://github.com/Arrow-Markets-Research/openmargin/raw/main/arrow-markets.png"></p>
 
 ![Python](https://img.shields.io/badge/python-v3.8+-green.svg)
-![Version](https://img.shields.io/badge/version-0.0.1-red.svg)
+![Version](https://img.shields.io/badge/version-0.0.3-red.svg)
 ![License](https://img.shields.io/badge/license-GNU-blue.svg)
 
 # Open Margin
 
 Arrow Markets open source repository to calculate margin requirements for risky asset portfolios including crypto options portfolios.
 
 ## Overview
 
-This repository includes a simplified version of the proprietary Arrow Markets margin calculator. <br />
-It uses VAR/CVAR methodology to compute the necessary margin required for a portfolio of BTC or ETH options. <br />
-Negative values refer to the cash margin needed for a given portfolio, while positive margin values count as credits. <br />
-For further details, please refer to the white paper ["Automated Margin Systems in Practice"](https://drive.google.com/file/d/12iX75pEvrZvwky-O8z6F1PeO65duMdyJ/view?usp=drive_link)
+This repository includes a simplified version of the proprietary Arrow Markets margin calculator. It uses VAR/CVAR methodology to compute the necessary margin required for a portfolio of BTC or ETH options. <br />
+Negative values refer to the cash margin needed for a given portfolio, while positive margin values count as credits. For further details, please refer to the white paper ["Automated Margin Systems in Practice"](https://drive.google.com/file/d/1y_113sCg4kOkU8lRDnyRjCovNpDMLNcM/view?usp=drive_link)
 
 ## Installation
 
 ```bash
 pip install openmargin
 ```
```

