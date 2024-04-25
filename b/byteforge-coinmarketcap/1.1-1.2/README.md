# Comparing `tmp/byteforge_coinmarketcap-1.1.tar.gz` & `tmp/byteforge_coinmarketcap-1.2.tar.gz`

## Comparing `byteforge_coinmarketcap-1.1.tar` & `byteforge_coinmarketcap-1.2.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.1/MANIFEST
--rwxr-xr-x   0        0        0      140 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.1/build_publish.sh
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.1/requirements.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.1/coinmarketcap/__init__.py
--rwxr-xr-x   0        0        0     3680 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.1/coinmarketcap/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.1/coinmarketcap/types/__init__.py
--rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.1/coinmarketcap/types/token_state.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.1/coinmarketcap/v1/cryptocurrency/listings/common.py
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.1/coinmarketcap/v1/cryptocurrency/listings/latest.py
--rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.1/coinmarketcap/v2/cryptocurrency/quotes/historical.py
--rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.1/doc/coinmarketcap.png
--rw-r--r--   0        0        0    21711 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.1/doc/coinmarketcap_original.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.1/tests/__init__.py
--rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.1/tests/test_coinmarketcap.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.1/.gitignore
--rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.1/LICENSE
--rw-r--r--   0        0        0    11254 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.1/README.md
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.1/pyproject.toml
--rw-r--r--   0        0        0    24267 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.1/PKG-INFO
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/MANIFEST
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/requirements.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/coinmarketcap/__init__.py
+-rwxr-xr-x   0        0        0     3946 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/coinmarketcap/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/coinmarketcap/types/__init__.py
+-rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/coinmarketcap/types/token_state.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/coinmarketcap/v1/cryptocurrency/listings/common.py
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/coinmarketcap/v1/cryptocurrency/listings/latest.py
+-rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/coinmarketcap/v2/cryptocurrency/quotes/historical.py
+-rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/doc/coinmarketcap.png
+-rw-r--r--   0        0        0    21711 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/doc/coinmarketcap_original.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/tests/__init__.py
+-rw-r--r--   0        0        0     6894 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/tests/test_coinmarketcap.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/.gitignore
+-rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/LICENSE
+-rw-r--r--   0        0        0    11588 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/README.md
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/pyproject.toml
+-rw-r--r--   0        0        0    24601 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.2/PKG-INFO
```

### Comparing `byteforge_coinmarketcap-1.1/coinmarketcap/core.py` & `byteforge_coinmarketcap-1.2/coinmarketcap/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import sys
 import json
 import requests
 import tempfile
+import time
 import requests_cache
-from typing import List
+from typing import Optional, List
 
 from .types.token_state import TokenState, Quote
 from .v2.cryptocurrency.quotes.historical import _quotes_historical_v2
 from .v1.cryptocurrency.listings.latest import _listings_latest
 from .v1.cryptocurrency.listings.common import SortOption, AuxFields, SortDir, FilterOptions
 
 class Market(object):
@@ -60,21 +61,28 @@
 				return response_object.json()
 			else:
 				raise Exception(f"Server returned {response_object.status_code} - {response_object.text}")
 		except Exception as e:
 			raise e
 
 	def quotes_historical(self,
-					   ticker: str,
-					   timestamp_start: int,
-					   timestamp_end: int,
-					   interval: str = '24h',
-					   convert: List[str] = ['USD']) -> List[TokenState]:
+						  id: Optional[str] = None,
+						  ticker: Optional[str] = None,
+						  timestamp_start: Optional[int] = int(time.time()) - 60*60*24,
+						  timestamp_end: Optional[int] = int(time.time()),
+						  interval: str = 'hourly',
+						  convert: List[str] = ['USD']) -> List[TokenState]:
 		
-		return _quotes_historical_v2(self, ticker, timestamp_start, timestamp_end, interval, convert)
+		return _quotes_historical_v2(self,
+							   id=id,
+							   ticker=ticker,
+							   timestamp_start=timestamp_start,
+							   timestamp_end=timestamp_end,
+							   interval=interval,
+							   convert=convert)
 
 	def listings_latest(self, sort_by: SortOption = SortOption.MARKET_CAP, 
 					sort_dir: SortDir = SortDir.DESC, 
 					start: int = 1, 
 					limit: int = 100, 
 					convert: List[str] = ['USD'],
 					aux_fields: AuxFields = None,
```

### Comparing `byteforge_coinmarketcap-1.1/coinmarketcap/types/token_state.py` & `byteforge_coinmarketcap-1.2/coinmarketcap/types/token_state.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,14 +39,20 @@
     market_cap_by_total_supply: Optional[float] = None
     volume_7d: Optional[float] = None
     total_supply: Optional[float] = None
     circulating_supply: Optional[float] = None
 
     @staticmethod
     def from_dict(currency: str, dct_quote_data: Dict) -> 'Quote':
+
+        # insure integers are handled as floats (so 1 becomes 1.0)
+        dct_quote_data['price'] = float(dct_quote_data['price'])
+        dct_quote_data['market_cap'] = float(dct_quote_data['market_cap'])
+
+
         # Handle both 'last_updated' and 'timestamp' for the last_updated field
         if 'last_updated' in dct_quote_data:
             last_updated_str = dct_quote_data['last_updated']
         elif 'timestamp' in dct_quote_data:
             last_updated_str = dct_quote_data['timestamp']
         else:
             raise ValueError("Payload must contain either 'last_updated' or 'timestamp' field.")
```

### Comparing `byteforge_coinmarketcap-1.1/coinmarketcap/v1/cryptocurrency/listings/common.py` & `byteforge_coinmarketcap-1.2/coinmarketcap/v1/cryptocurrency/listings/common.py`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.1/coinmarketcap/v1/cryptocurrency/listings/latest.py` & `byteforge_coinmarketcap-1.2/coinmarketcap/v1/cryptocurrency/listings/latest.py`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.1/coinmarketcap/v2/cryptocurrency/quotes/historical.py` & `byteforge_coinmarketcap-1.2/coinmarketcap/v2/cryptocurrency/quotes/historical.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,49 +19,63 @@
     }
 
     # Check if the interval is in one of the allowed sets
     if interval not in calendar_intervals and interval not in relative_intervals:
         # If not, raise a ValueError with a message about the invalid interval
         raise ValueError(f"Invalid interval: '{interval}'. Please provide a valid interval.")
 
-
-def _quotes_historical_v2(market, 
-						  ticker: str, 
-						  timestamp_start: Optional[int], 
-						  timestamp_end: Optional[int],
+def _quotes_historical_v2(market,
+						  id: Optional[str] = None,
+						  ticker: Optional[str] = None,
+						  timestamp_start: Optional[int] = int(time.time()) - 60*60*24,
+						  timestamp_end: Optional[int] = int(time.time()),
 						  interval: str = 'hourly',
 						  convert: List[str] = ['USD']) -> List[TokenState]:
 
+	if not id and not ticker:
+		raise ValueError('Either id or ticker must be provided')
+
 	# Check if the start timestamp is greater than the end timestamp
 	if timestamp_start > timestamp_end:
 		raise ValueError('The start timestamp occurr before than the end timestamp')
 
 	# Check if the interval is valid
 	_validate_interval(interval)
 
 	# validate convert
 	if (len(convert) > 3):
 		raise ValueError('The convert list must have a maximum of 3 elements')
 
 	params = {
-		'symbol': ticker,
 		'time_start': timestamp_start,
 		'time_end': timestamp_end,
 		'interval': interval,
 		'convert': ','.join(convert)
 	}
+
+	# use id if provided, otherwise use ticker
+	if id:
+		params['id'] = id
+	else:
+		params['symbol'] = ticker
 		
 	response = market._request('v2/cryptocurrency/quotes/historical', params=params)
 
 	lst_token_states = []
 
-	# weird structure, we have to drill down into the quotes object for our ticker,
-	# we call this the quote summary because it's the quotes, plus some extra
-	# meta data we can extract for the TokenState object
-	dct_quote_summary = response['data'][ticker][0]
+	if id:
+		# if we are querying by id, we get a simpler (although not completely simple)
+		# structure to parse
+		dct_quote_summary = response['data']
+	else:
+		# if we query by ticker we get a differeint weird structure, we have to 
+		# drill down into the quotes object for our ticker, we call this the quote 
+	    # summary because it's the quotes, plus some extra
+		# meta data we can extract for the TokenState object
+		dct_quote_summary = response['data'][ticker][0]
 
 	# and we also get some general meta-data that can go into the TokenState object
 	id = dct_quote_summary['id']
 	name = dct_quote_summary['name']
 	symbol = dct_quote_summary['symbol']
 	is_active = dct_quote_summary['is_active'] == 1
 	is_fiat = dct_quote_summary['is_fiat'] == 1
```

### Comparing `byteforge_coinmarketcap-1.1/doc/coinmarketcap.png` & `byteforge_coinmarketcap-1.2/doc/coinmarketcap.png`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.1/doc/coinmarketcap_original.png` & `byteforge_coinmarketcap-1.2/doc/coinmarketcap_original.png`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.1/tests/test_coinmarketcap.py` & `byteforge_coinmarketcap-1.2/tests/test_coinmarketcap.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,15 +11,65 @@
 def coinmarketcap_instance():
     # You can initialize your CoinMarketCap instance with your API key here if needed
     api_key=API_KEY = os.environ.get('COIN_MARKET_CAP_API_KEY')
     coinmarketcap_instance = Market(api_key=api_key, debug_mode=True)
     yield coinmarketcap_instance
 
 
-def test_cryptocurrency_quotes_historical(coinmarketcap_instance):
+def test_cryptocurrency_quotes_historical_with_id(coinmarketcap_instance):
+
+    timestamp_now = int(time.time())
+    timestamp_1_day_ago = timestamp_now - 60*60*24
+
+    # Make the API call
+    token_states = coinmarketcap_instance.quotes_historical(
+        id="1",
+        timestamp_start=timestamp_1_day_ago,
+        timestamp_end=timestamp_now,
+        interval='1h',
+        convert=['USD', 'BTC']
+    )
+
+    # Check if the response is a list and contains at least one item
+    assert isinstance(token_states, list)
+    assert len(token_states) >= 1
+
+    # Check the attributes of the first token state
+    token_state = token_states[0]
+    assert isinstance(token_state.id, int)
+    assert isinstance(token_state.name, str)
+    assert isinstance(token_state.symbol, str)
+    assert isinstance(token_state.last_updated, datetime)
+    assert isinstance(token_state.timestamp, int)
+    assert isinstance(token_state.is_active, bool)
+    assert isinstance(token_state.is_fiat, bool)
+    assert isinstance(token_state.quote_map, dict)
+
+    # Check the attributes of the USD quote
+    quote = token_state.quote_map['USD']
+    assert isinstance(quote.price, float)
+    assert isinstance(quote.volume_24h, float)
+    assert isinstance(quote.percent_change_1h, float)
+    assert isinstance(quote.percent_change_24h, float)
+    assert isinstance(quote.percent_change_7d, float)
+    assert isinstance(quote.market_cap, float)
+    assert isinstance(quote.last_updated, datetime)
+
+    # Check the attributes of the BTC quote
+    quote = token_state.quote_map['BTC']
+    assert isinstance(quote.price, float)
+    assert isinstance(quote.volume_24h, float)
+    assert isinstance(quote.percent_change_1h, float)
+    assert isinstance(quote.percent_change_24h, float)
+    assert isinstance(quote.percent_change_7d, float)
+    assert isinstance(quote.market_cap, float)
+    assert isinstance(quote.last_updated, datetime)
+
+
+def test_cryptocurrency_quotes_historical_with_ticker(coinmarketcap_instance):
     
     timestamp_now = int(time.time())
     timestamp_1_day_ago = timestamp_now - 60*60*24
     
     # Make the API call
     token_states = coinmarketcap_instance.quotes_historical(
         ticker='ETH',
```

### Comparing `byteforge_coinmarketcap-1.1/LICENSE` & `byteforge_coinmarketcap-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.1/README.md` & `byteforge_coinmarketcap-1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,16 @@
 # BNB BNB 369.2725354702457
 # Solana SOL 103.68827889524766
 ```
 ### The `convert` parameter
 
 The `convert` parameter enhances your ability to receive cryptocurrency quotes in multiple currencies simultaneously. This feature is especially useful for comparing market values across different fiat and cryptocurrencies, allowing up to three currency conversions in a single request.
 
+**Please Note:** You’ll need a hobbyist account or higher to do more than one conversion at a time.
+
 Here's how you can retrieve the latest listings and obtain quotes in USD and BTC for the top 5 cryptocurrencies by market capitalization:
 
 ```python
 # Fetch listings with market cap sort, limited to the top 5, converting quotes to USD and BTC
 tokens = coinmarketcap.listings_latest(sort_by=SortOption.MARKET_CAP, limit=5, convert=['USD', 'BTC'])
 
 # Iterate through each token to display its name, symbol, and quotes in BTC and USD
@@ -185,15 +187,15 @@
 for token in tokens:
     print(f"{token.name} ({token.symbol}) - CMC Rank: {token.cmc_rank}, Market Pairs: {token.num_market_pairs}")
 ```
 
 ## Usage: API quotes_historical
 
 
-The `quotes_historical` method facilitates fetching historical quotes for a specific cryptocurrency over a given time range. This feature allows for detailed analysis of cryptocurrency value trends over time in different fiat or cryptocurrencies.
+The `quotes_historical` method facilitates fetching historical quotes for a specific cryptocurrency over a given time range. This feature allows for detailed analysis of cryptocurrency value trends over time in different fiat or cryptocurrencies.  You can query either directly by ticker using the ```ticker``` paramater or using the ```id``` parameter and supply the coinmarketcap id (cmc_id).  Using the cmd_id can avoid edge cases when multiple assets share the same ticker.
 
 This API requires a 'Hobbyist' or higher tier CMC subscription.
 
 ### Example Usage
 
 ```python
 from byteforge_coinmarketcap import Market
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `byteforge_coinmarketcap-1.1/pyproject.toml` & `byteforge_coinmarketcap-1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "byteforge-coinmarketcap"
-version = "1.1"
+version = "1.2"
 description = "Python SDK for the coinmarketcap.com API."
 readme = "README.md"
 license = { file="LICENSE" }
 keywords = ["cryptocurrency", "API", "coinmarketcap", "BTC", "Bitcoin", "LTC", "Litecoin", "XRP", "Ripple", "ETH", "Ethereum"]
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `byteforge_coinmarketcap-1.1/PKG-INFO` & `byteforge_coinmarketcap-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: byteforge-coinmarketcap
-Version: 1.1
+Version: 1.2
 Summary: Python SDK for the coinmarketcap.com API.
 Project-URL: Homepage, https://github.com/jmazzahacks/byteforge-coinmarketcap/
 Project-URL: Issues, https://github.com/jmazzahacks/byteforge-coinmarketcap/issues
 Author: Jason Byteforgia
 License:                              Apache License
                                Version 2.0, January 2004
                             http://www.apache.org/licenses/
@@ -272,14 +272,16 @@
 # BNB BNB 369.2725354702457
 # Solana SOL 103.68827889524766
 ```
 ### The `convert` parameter
 
 The `convert` parameter enhances your ability to receive cryptocurrency quotes in multiple currencies simultaneously. This feature is especially useful for comparing market values across different fiat and cryptocurrencies, allowing up to three currency conversions in a single request.
 
+**Please Note:** You’ll need a hobbyist account or higher to do more than one conversion at a time.
+
 Here's how you can retrieve the latest listings and obtain quotes in USD and BTC for the top 5 cryptocurrencies by market capitalization:
 
 ```python
 # Fetch listings with market cap sort, limited to the top 5, converting quotes to USD and BTC
 tokens = coinmarketcap.listings_latest(sort_by=SortOption.MARKET_CAP, limit=5, convert=['USD', 'BTC'])
 
 # Iterate through each token to display its name, symbol, and quotes in BTC and USD
@@ -404,15 +406,15 @@
 for token in tokens:
     print(f"{token.name} ({token.symbol}) - CMC Rank: {token.cmc_rank}, Market Pairs: {token.num_market_pairs}")
 ```
 
 ## Usage: API quotes_historical
 
 
-The `quotes_historical` method facilitates fetching historical quotes for a specific cryptocurrency over a given time range. This feature allows for detailed analysis of cryptocurrency value trends over time in different fiat or cryptocurrencies.
+The `quotes_historical` method facilitates fetching historical quotes for a specific cryptocurrency over a given time range. This feature allows for detailed analysis of cryptocurrency value trends over time in different fiat or cryptocurrencies.  You can query either directly by ticker using the ```ticker``` paramater or using the ```id``` parameter and supply the coinmarketcap id (cmc_id).  Using the cmd_id can avoid edge cases when multiple assets share the same ticker.
 
 This API requires a 'Hobbyist' or higher tier CMC subscription.
 
 ### Example Usage
 
 ```python
 from byteforge_coinmarketcap import Market
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

