# Comparing `tmp/py_alpaca_api-0.5.4.tar.gz` & `tmp/py_alpaca_api-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_alpaca_api-0.5.4.tar", max compression
+gzip compressed data, was "py_alpaca_api-0.5.6.tar", max compression
```

## Comparing `py_alpaca_api-0.5.4.tar` & `py_alpaca_api-0.5.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1066 2024-05-19 01:27:26.322892 py_alpaca_api-0.5.4/LICENSE
--rw-r--r--   0        0        0    16791 2024-05-19 11:02:34.884010 py_alpaca_api-0.5.4/README.md
--rw-r--r--   0        0        0        0 2024-05-19 01:27:26.322892 py_alpaca_api-0.5.4/py_alpaca_api/__init__.py
--rw-r--r--   0        0        0     2490 2024-05-19 20:03:29.845131 py_alpaca_api-0.5.4/py_alpaca_api/alpaca.py
--rw-r--r--   0        0        0        0 2024-05-19 01:27:26.322892 py_alpaca_api-0.5.4/py_alpaca_api/src/__init__.py
--rw-r--r--   0        0        0     4672 2024-05-20 23:00:54.419417 py_alpaca_api-0.5.4/py_alpaca_api/src/account.py
--rw-r--r--   0        0        0     3789 2024-05-20 23:00:54.419417 py_alpaca_api-0.5.4/py_alpaca_api/src/asset.py
--rw-r--r--   0        0        0    20726 2024-05-20 02:57:54.840513 py_alpaca_api-0.5.4/py_alpaca_api/src/data_classes.py
--rw-r--r--   0        0        0     7775 2024-05-20 23:00:54.419417 py_alpaca_api-0.5.4/py_alpaca_api/src/history.py
--rw-r--r--   0        0        0     2141 2024-05-20 23:00:54.419417 py_alpaca_api-0.5.4/py_alpaca_api/src/market.py
--rw-r--r--   0        0        0    13186 2024-05-20 23:00:54.419417 py_alpaca_api-0.5.4/py_alpaca_api/src/order.py
--rw-r--r--   0        0        0    14989 2024-05-20 02:57:54.840513 py_alpaca_api-0.5.4/py_alpaca_api/src/position.py
--rw-r--r--   0        0        0     8824 2024-05-21 00:28:44.038648 py_alpaca_api-0.5.4/py_alpaca_api/src/screener.py
--rw-r--r--   0        0        0    14951 2024-05-20 02:57:54.840513 py_alpaca_api-0.5.4/py_alpaca_api/src/watchlist.py
--rw-r--r--   0        0        0     1344 2024-05-21 00:28:44.038648 py_alpaca_api-0.5.4/pyproject.toml
--rw-r--r--   0        0        0    17593 1970-01-01 00:00:00.000000 py_alpaca_api-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-19 01:27:26.322892 py_alpaca_api-0.5.6/LICENSE
+-rw-r--r--   0        0        0    16791 2024-05-19 11:02:34.884010 py_alpaca_api-0.5.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-19 01:27:26.322892 py_alpaca_api-0.5.6/py_alpaca_api/__init__.py
+-rw-r--r--   0        0        0     2490 2024-05-22 22:57:11.657657 py_alpaca_api-0.5.6/py_alpaca_api/alpaca.py
+-rw-r--r--   0        0        0        0 2024-05-22 22:57:11.657657 py_alpaca_api-0.5.6/py_alpaca_api/src/__init__.py
+-rw-r--r--   0        0        0     4672 2024-05-20 23:00:54.419417 py_alpaca_api-0.5.6/py_alpaca_api/src/account.py
+-rw-r--r--   0        0        0     3789 2024-05-22 22:57:11.657657 py_alpaca_api-0.5.6/py_alpaca_api/src/asset.py
+-rw-r--r--   0        0        0    20726 2024-05-20 02:57:54.840513 py_alpaca_api-0.5.6/py_alpaca_api/src/data_classes.py
+-rw-r--r--   0        0        0     8341 2024-05-23 02:44:37.096464 py_alpaca_api-0.5.6/py_alpaca_api/src/history.py
+-rw-r--r--   0        0        0     2141 2024-05-20 23:00:54.419417 py_alpaca_api-0.5.6/py_alpaca_api/src/market.py
+-rw-r--r--   0        0        0    13186 2024-05-22 22:57:11.657657 py_alpaca_api-0.5.6/py_alpaca_api/src/order.py
+-rw-r--r--   0        0        0    14989 2024-05-20 02:57:54.840513 py_alpaca_api-0.5.6/py_alpaca_api/src/position.py
+-rw-r--r--   0        0        0     8824 2024-05-22 22:57:11.657657 py_alpaca_api-0.5.6/py_alpaca_api/src/screener.py
+-rw-r--r--   0        0        0    14951 2024-05-20 02:57:54.840513 py_alpaca_api-0.5.6/py_alpaca_api/src/watchlist.py
+-rw-r--r--   0        0        0     1344 2024-05-23 02:45:38.106461 py_alpaca_api-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0    17593 1970-01-01 00:00:00.000000 py_alpaca_api-0.5.6/PKG-INFO
```

### Comparing `py_alpaca_api-0.5.4/LICENSE` & `py_alpaca_api-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.5.4/README.md` & `py_alpaca_api-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.5.4/py_alpaca_api/alpaca.py` & `py_alpaca_api-0.5.6/py_alpaca_api/alpaca.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.5.4/py_alpaca_api/src/account.py` & `py_alpaca_api-0.5.6/py_alpaca_api/src/account.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.5.4/py_alpaca_api/src/asset.py` & `py_alpaca_api-0.5.6/py_alpaca_api/src/asset.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.5.4/py_alpaca_api/src/data_classes.py` & `py_alpaca_api-0.5.6/py_alpaca_api/src/data_classes.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.5.4/py_alpaca_api/src/history.py` & `py_alpaca_api-0.5.6/py_alpaca_api/src/history.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,191 +1,149 @@
 import json
+from collections import defaultdict
 from typing import Dict
 
 import pandas as pd
 import requests
 
 from .asset import Asset
+from .data_classes import AssetClass
 
 
 class History:
     def __init__(self, data_url: str, headers: Dict[str, str], asset: Asset) -> None:
-        """Initialize History class
-
-        Parameters:
-        ___________
-        data_url: str
-                Alpaca Data API URL required
-
-        headers: object
-                API request headers required
-
-        asset: Asset
-                Asset object required
-
-        Raises:
-        _______
-        ValueError: If data URL is not provided
-
-        ValueError: If headers are not provided
-
-        ValueError: If asset is not provided
-        """  # noqa
+        """
+        Args:
+            data_url: A string representing the URL of the data.
+            headers: A dictionary containing the headers to be included in the request.
+            asset: An instance of the Asset class representing the asset.
 
+        """
         self.data_url = data_url
         self.headers = headers
         self.asset = asset
 
-    ############################
-    # Get Stock Historical Data
-    ############################
+    ###########################################
+    # ////// Get Stock Historical Data \\\\\\ #
+    ###########################################
     def get_stock_data(
         self,
-        symbol,
-        start,
-        end,
-        timeframe="1d",
-        feed="iex",
-        currency="USD",
-        limit=1000,
-        sort="asc",
-        adjustment="raw",
+        symbol: str,
+        start: str,
+        end: str,
+        timeframe: str = "1d",
+        feed: str = "sip",
+        currency: str = "USD",
+        limit: int = 1000,
+        sort: str = "asc",
+        adjustment: str = "raw",
     ) -> pd.DataFrame:
-        """Get historical stock data from Alpaca API
-
-        Parameters:
-        ___________
-        symbol: str
-                Stock symbol required
+        """
+        Args:
+            symbol: The stock symbol to fetch data for.
+            start: The start date for historical data in the format "YYYY-MM-DD".
+            end: The end date for historical data in the format "YYYY-MM-DD".
+            timeframe: The timeframe for the historical data. Default is "1d".
+            Possible values are "1m", "5m", "15m", "30m", "1h", "4h", "1d", "1w", or "1M".
+            feed: The data feed source. Default is "sip".
+            currency: The currency for historical data. Default is "USD".
+            limit: The number of data points to fetch. Default is 1000.
+            sort: The sort order for the data. Default is "asc".
+            adjustment: The adjustment for historical data. Default is "raw".
 
-        start: str
-                Start date for historical data required, format: YYYY-MM-DD
+        Returns:
+            A pandas DataFrame containing the historical stock data for the given symbol and time range.
 
-        end: str
-                End date for historical data required, format: YYYY-MM-DD
+        Raises:
+            ValueError: If the given timeframe is not one of the allowed values.
 
-        timeframe: str
-                Timeframe for historical data, default: 1d
-                Choices: "1m", "5m", "15m", "30m", "1h", "4h", "1d", "1w", "1m"
+        """
 
-        feed: str
-                Data feed source, default: iex
-                Choices: "iex", "sip", "otc"
+        self.check_if_stock(symbol)
 
-        currency: str
-                Currency for historical data, default: USD
+        # URL for historical stock data request
+        url = f"{self.data_url}/stocks/{symbol}/bars"
+        # Set timeframe
+        timeframe_mapping: dict = {
+            "1m": "1Min",
+            "5m": "5Min",
+            "15m": "15Min",
+            "30m": "30Min",
+            "1h": "1Hour",
+            "4h": "4Hour",
+            "1d": "1Day",
+            "1w": "1Week",
+            "1M": "1Month",
+        }
 
-        limit: int
-                Limit number of data points, default: 1000
-                The maximum number of data points to return in the response.
+        if timeframe not in timeframe_mapping:
+            raise ValueError('Invalid timeframe. Must be "1m", "5m", "15m", "30m", "1h", "4h", "1d", "1w", or "1M"')
 
-        sort: str
-                Sort order, default: asc, Choices: "asc", "desc"
+        # Parameters for historical stock data request
+        params = {
+            "timeframe": timeframe_mapping[timeframe],  # Timeframe for historical data, default: 1d
+            "start": start,  # Start date for historical data
+            "end": end,  # End date for historical data
+            "currency": currency,  # Currency for historical data, default: USD
+            "limit": limit,  # Limit number of data points, default: 1000
+            "adjustment": adjustment,  # Adjustment for historical data, default: raw
+            "feed": feed,  # Data feed source, default: iex
+            "sort": sort,  # Sort order, default: asc
+        }
+        symbol_data = self.get_historical_data(symbol, url, params)
+        bar_data_df = self.preprocess_data(symbol_data, symbol)
+        return bar_data_df
 
-        adjustment: str
-                Adjustment for historical data, default: raw
-                Choices: "raw", "split", "dividend", "merger", "all"
+    ###########################################
+    # /////// Check if Asset is Stock \\\\\\\ #
+    ###########################################
+    def check_if_stock(self, symbol: str) -> AssetClass:
+        """Check if asset is stock
+        Args:
+            symbol: The symbol of the asset to be checked.
 
         Returns:
-        ________
-        pd.DataFrame: Historical stock data as a DataFrame
+            AssetClass: The asset information for the given symbol.
 
         Raises:
-        _______
-        ValueError: If the response is not successful
-
-        ValueError: If the asset is not a stock
-
-        ValueError: If no data is available
-
-        ValueError: If invalid timeframe is provided
-
-        Example:
-        ________
-        >>> from py_alpaca_api.alpaca import PyAlpacaApi
-            api = PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
-            stock_data = api.history.get_stock_data(symbol="AAPL", start="2021-01-01", end="2021-12-31", timeframe="1d")
-            print(stock_data)
-
-        symbol       date    open    high     low   close    volume  trade_count     vwap
-        AAPL    2021-01-04  133.52  133.61  126.76  129.41  143301887      1009115  130.914
-        AAPL    2021-01-05  128.89  131.74  128.43  131.01   97664898       678471  130.573
-        AAPL    2021-01-06  127.72  131.05  126.38  126.60  155087970      1135783  128.073
-        AAPL    2021-01-07  128.36  131.63  127.86  130.92  109578157       791297  129.918
-        AAPL    2021-01-08  132.43  132.63  130.23  132.05  105158245       743315  131.573
-        ...            ...     ...     ...     ...     ...        ...          ...      ...
-        AAPL    2021-12-23  176.69  177.36  175.55  177.36   30925200       123456  176.423
-        AAPL    2021-12-27  177.41  179.15  177.36  179.15   36254100       145236  178.423
-        AAPL    2021-12-28  179.15  179.25  177.36  177.36   30925200       123456  178.423
-        AAPL    2021-12-29  177.36  179.15  177.36  179.15   36254100       145236  178.423
-        AAPL    2021-12-30  179.15  179.25  177.36  177.36   30925200       123456  178.423
-
-        [252 rows x 9 columns]
-        """  # noqa
-
+            ValueError: If there is an error getting the asset information or if the asset is not a stock.
+        """
         # Get asset information for the symbol
         try:
             asset = self.asset.get(symbol)
         # Raise exception if failed to get asset information
         except Exception as e:
             raise ValueError(e)
         else:
             # Check if asset is a stock
             if asset.asset_class != "us_equity":
                 # Raise exception if asset is not a stock
                 raise ValueError(f"{symbol} is not a stock.")
-        # URL for historical stock data request
-        url = f"{self.data_url}/stocks/{symbol}/bars"
-        # Set timeframe
-        match timeframe:
-            case "1m":
-                timeframe = "1Min"
-            case "5m":
-                timeframe = "5Min"
-            case "15m":
-                timeframe = "15Min"
-            case "30m":
-                timeframe = "30Min"
-            case "1h":
-                timeframe = "1Hour"
-            case "4h":
-                timeframe = "4Hour"
-            case "1d":
-                timeframe = "1Day"
-            case "1w":
-                timeframe = "1Week"
-            case "1m":
-                timeframe = "1Month"
-            case _:
-                # Raise exception if invalid timeframe is provided
-                raise ValueError('Invalid timeframe. Must be "1m", "5m", "15m", "30m", "1h", "4h", "1d", "1w", or "1m"')
-        # Parameters for historical stock data request
-        params = {
-            "timeframe": timeframe,  # Timeframe for historical data, default: 1d
-            "start": start,  # Start date for historical data
-            "end": end,  # End date for historical data
-            "currency": currency,  # Currency for historical data, default: USD
-            "limit": limit,  # Limit number of data points, default: 1000
-            "adjustment": adjustment,  # Adjustment for historical data, default: raw
-            "feed": feed,  # Data feed source, default: iex
-            "sort": sort,  # Sort order, default: asc
-        }
-        # Get historical stock data from Alpaca API
-        response = requests.get(url, headers=self.headers, params=params)
-        # Check if response is successful
-        if response.status_code != 200:
-            # Raise exception if response is not successful
-            raise Exception(json.loads(response.text)["message"])
+        return asset
+
+    ###########################################
+    # /////////// PreProcess Data \\\\\\\\\\\ #
+    ###########################################
+    @staticmethod
+    def preprocess_data(symbol_data: list[defaultdict], symbol: str) -> pd.DataFrame:
+        """Prepross data
+        Preprocesses the given symbol data by converting it to a pandas DataFrame and performing various
+        data transformations.
+
+        Args:
+            symbol_data: A list of defaultdict objects representing the JSON response data.
+            symbol: A string representing the symbol or ticker for the stock data.
+
+        Returns:
+            A pandas DataFrame containing the preprocessed historical stock data.
+
+        """
         # Convert JSON response to dictionary
-        res_json = json.loads(response.text)["bars"]
-        # Check if data is available
-        if not res_json:
-            raise ValueError(f"No data available for {symbol}.")
-        # Normalize JSON response and convert to DataFrame
-        bar_data_df = pd.json_normalize(res_json)
+        bar_data_df = pd.DataFrame(symbol_data)
+
         # Add symbol column to DataFrame
         bar_data_df.insert(0, "symbol", symbol)
         # Reformat date column
         bar_data_df["t"] = pd.to_datetime(bar_data_df["t"].replace("[A-Za-z]", " ", regex=True))
         # Rename columns for consistency
         bar_data_df.rename(
             columns={
@@ -212,7 +170,48 @@
                 "vwap": "float",
                 "trade_count": "int",
                 "volume": "int",
             }
         )
         # Return historical stock data as a DataFrame
         return bar_data_df
+
+    ###########################################
+    # ///////// Get Historical Data \\\\\\\\\ #
+    ###########################################
+    def get_historical_data(self, symbol: str, url: str, params: dict) -> list[defaultdict]:
+        """Get historical stock data
+        Args:
+            symbol (str): The symbol of the stock or asset for which historical data is being fetched.
+            url (str): The URL of the API endpoint from where the historical data is being fetched.
+            params (dict): Additional parameters to be passed along with the API request.
+
+        Returns:
+            list: A list of dictionaries containing the historical data for the specified symbol.
+
+        Raises:
+            Exception: If the API response status code is not 200, an exception is raised with the error message.
+
+
+        This function fetches historical data for a given symbol by making requests to the specified API endpoint.
+        It uses a page token to paginate through the response data and retrieves all available historical bars.
+
+        Example usage:
+            symbol = "AAPL"
+            url = "https://api.example.com/historical"
+            params = {"start_date": "2021-01-01", "end_date": "2021-01-31"}
+
+            historical_data = get_historical_data(symbol, url, params)
+        """
+        page_token = None
+        symbols_data = defaultdict(list)
+        while True:
+            params["page_token"] = page_token
+            response = requests.get(url, headers=self.headers, params=params)
+            if response.status_code != 200:
+                raise Exception(json.loads(response.text)["message"])
+            res_data = response.json()
+            symbols_data[symbol].extend(res_data.get("bars", []))
+            page_token = res_data.get("next_page_token", "")
+            if not page_token:
+                break
+        return symbols_data[symbol]
```

### Comparing `py_alpaca_api-0.5.4/py_alpaca_api/src/market.py` & `py_alpaca_api-0.5.6/py_alpaca_api/src/market.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.5.4/py_alpaca_api/src/order.py` & `py_alpaca_api-0.5.6/py_alpaca_api/src/order.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.5.4/py_alpaca_api/src/position.py` & `py_alpaca_api-0.5.6/py_alpaca_api/src/position.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.5.4/py_alpaca_api/src/screener.py` & `py_alpaca_api-0.5.6/py_alpaca_api/src/screener.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.5.4/py_alpaca_api/src/watchlist.py` & `py_alpaca_api-0.5.6/py_alpaca_api/src/watchlist.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.5.4/pyproject.toml` & `py_alpaca_api-0.5.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-alpaca-api"
-version = "0.5.4"
+version = "0.5.6"
 description = "Python package, for communicating with Alpaca Markets REST API."
 authors = ["TexasCoding <jeff10278@me.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/TexasCoding/py-alpaca-api"
 repository = "https://github.com/TexasCoding/py-alpaca-api"
 documentation = "https://py-alpaca-api.readthedocs.io/en/latest/"
```

### Comparing `py_alpaca_api-0.5.4/PKG-INFO` & `py_alpaca_api-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-alpaca-api
-Version: 0.5.4
+Version: 0.5.6
 Summary: Python package, for communicating with Alpaca Markets REST API.
 Home-page: https://github.com/TexasCoding/py-alpaca-api
 License: MIT
 Keywords: alpaca,python
 Author: TexasCoding
 Author-email: jeff10278@me.com
 Requires-Python: >=3.12,<4.0
```

