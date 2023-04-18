# Comparing `tmp/pigeonapi-python-client-0.10.tar.gz` & `tmp/pigeonapi-python-client-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pigeonapi-python-client-0.10.tar", last modified: Tue Apr 18 17:20:50 2023, max compression
+gzip compressed data, was "dist/pigeonapi-python-client-0.9.tar", last modified: Fri Nov  4 19:51:00 2022, max compression
```

## Comparing `pigeonapi-python-client-0.10.tar` & `pigeonapi-python-client-0.9.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-18 17:20:50.000000 pigeonapi-python-client-0.10/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1053 2022-11-04 13:54:35.000000 pigeonapi-python-client-0.10/LICENSE
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1796 2023-04-18 17:20:50.000000 pigeonapi-python-client-0.10/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1136 2023-04-18 14:23:10.000000 pigeonapi-python-client-0.10/README.md
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-18 17:20:50.000000 pigeonapi-python-client-0.10/pigeon/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       93 2022-11-04 13:54:35.000000 pigeonapi-python-client-0.10/pigeon/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1174 2023-04-18 14:04:36.000000 pigeonapi-python-client-0.10/pigeon/config.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      599 2023-04-18 12:51:29.000000 pigeonapi-python-client-0.10/pigeon/exceptions.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-18 17:20:50.000000 pigeonapi-python-client-0.10/pigeon/rest/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      136 2022-11-04 13:54:35.000000 pigeonapi-python-client-0.10/pigeon/rest/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1291 2023-04-18 14:04:43.000000 pigeonapi-python-client-0.10/pigeon/rest/authenticator.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2982 2023-04-18 13:57:16.000000 pigeonapi-python-client-0.10/pigeon/rest/historical_candles.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5733 2023-04-18 13:55:55.000000 pigeonapi-python-client-0.10/pigeon/rest/intraday_candles.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-18 17:20:50.000000 pigeonapi-python-client-0.10/pigeon/websocket/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       45 2022-11-04 13:54:35.000000 pigeonapi-python-client-0.10/pigeon/websocket/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6371 2023-04-18 14:17:07.000000 pigeonapi-python-client-0.10/pigeon/websocket/websocket_client.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      270 2022-11-04 13:54:35.000000 pigeonapi-python-client-0.10/pigeon/websocket/websocket_default_functions.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-18 17:20:50.000000 pigeonapi-python-client-0.10/pigeonapi_python_client.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1796 2023-04-18 17:20:50.000000 pigeonapi-python-client-0.10/pigeonapi_python_client.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      550 2023-04-18 17:20:50.000000 pigeonapi-python-client-0.10/pigeonapi_python_client.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-04-18 17:20:50.000000 pigeonapi-python-client-0.10/pigeonapi_python_client.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       68 2023-04-18 17:20:50.000000 pigeonapi-python-client-0.10/pigeonapi_python_client.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        7 2023-04-18 17:20:50.000000 pigeonapi-python-client-0.10/pigeonapi_python_client.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-04-18 17:20:50.000000 pigeonapi-python-client-0.10/setup.cfg
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     1205 2023-04-17 20:57:58.000000 pigeonapi-python-client-0.10/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2022-11-04 19:51:00.000000 pigeonapi-python-client-0.9/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1478 2022-11-04 19:51:00.000000 pigeonapi-python-client-0.9/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      826 2022-11-04 13:54:35.000000 pigeonapi-python-client-0.9/README.md
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2022-11-04 19:51:00.000000 pigeonapi-python-client-0.9/pigeon/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       93 2022-11-04 13:54:35.000000 pigeonapi-python-client-0.9/pigeon/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1762 2022-11-04 19:40:03.000000 pigeonapi-python-client-0.9/pigeon/config.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      390 2022-11-04 14:53:23.000000 pigeonapi-python-client-0.9/pigeon/exceptions.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2022-11-04 19:51:00.000000 pigeonapi-python-client-0.9/pigeon/rest/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      136 2022-11-04 13:54:35.000000 pigeonapi-python-client-0.9/pigeon/rest/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1290 2022-11-04 14:32:52.000000 pigeonapi-python-client-0.9/pigeon/rest/authenticator.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3514 2022-11-04 13:54:35.000000 pigeonapi-python-client-0.9/pigeon/rest/historical_candles.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2826 2022-11-04 13:54:35.000000 pigeonapi-python-client-0.9/pigeon/rest/intraday_candles.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2022-11-04 19:51:00.000000 pigeonapi-python-client-0.9/pigeon/websocket/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       45 2022-11-04 13:54:35.000000 pigeonapi-python-client-0.9/pigeon/websocket/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6371 2022-11-04 19:42:22.000000 pigeonapi-python-client-0.9/pigeon/websocket/websocket_client.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      270 2022-11-04 13:54:35.000000 pigeonapi-python-client-0.9/pigeon/websocket/websocket_default_functions.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2022-11-04 19:51:00.000000 pigeonapi-python-client-0.9/pigeonapi_python_client.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1478 2022-11-04 19:51:00.000000 pigeonapi-python-client-0.9/pigeonapi_python_client.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      542 2022-11-04 19:51:00.000000 pigeonapi-python-client-0.9/pigeonapi_python_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2022-11-04 19:51:00.000000 pigeonapi-python-client-0.9/pigeonapi_python_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       51 2022-11-04 19:51:00.000000 pigeonapi-python-client-0.9/pigeonapi_python_client.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        7 2022-11-04 19:51:00.000000 pigeonapi-python-client-0.9/pigeonapi_python_client.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2022-11-04 19:51:00.000000 pigeonapi-python-client-0.9/setup.cfg
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     1204 2022-11-04 19:33:21.000000 pigeonapi-python-client-0.9/setup.py
```

### Comparing `pigeonapi-python-client-0.10/PKG-INFO` & `pigeonapi-python-client-0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 Metadata-Version: 2.1
 Name: pigeonapi-python-client
-Version: 0.10
+Version: 0.9
 Summary: Python package containing several classes and data for extracting and manipulating market and trading data.
 Home-page: https://github.com/BTG-Pactual-Solutions/pigeonapi-python-client
 Author: PigeonAPI powered by BTG Pactual Solutions
 License: UNKNOWN
 Description: # Pigeon
         
         Pigeon is a Python library to get Brazilian Financial Market Data.
         
         ## Installation
         
         ```bash
         pip3 install pigeonapi-python-client
         ```
         
-        ## Example - WebSocket Books
-        ```python
-        import pigeon
-        ws = pigeon.WebSocketClient(api_key='YOUR_API_KEY', ws_type='books', instruments=['PETR4', 'VALE3'])
-        ws.run(on_message=lambda message: print(message))
-        ```
-        ## Example - WebSocket Trades Delayed
+        ## Example - WebSocket
+        
         ```python
         import pigeon
-        ws = pigeon.WebSocketClient(api_key='YOUR_API_KEY', ws_type='trades', target='delayed', instruments=['PETR4', 'VALE3'])
+        
+        ws = pigeon.WebSocketClient(api_key='YOUR_API_KEY', instruments=['PETR4', 'VALE3'])
         ws.run(on_message=lambda message: print(message))
         ```
-        
         ## Example - IntradayCandles
+        
         ```python
         import pigeon
+        
         int_candles = pigeon.IntradayCandles(api_key='YOUR_API_KEY')
-        int_candles.get_intraday_candles(market_type='stocks', tickers=['PETR4', 'VALE3'], candle_period='1m', mode='relative', raw_data=True)
+        int_candles.get_intraday_candles(ticker='PETR4', candle_period='1m', mode='relative')
         ```
-        ## Example - Plot HistoricalCandles
+        ## Example - HistoricalCandles
+        
         ```python
-        import pigeon
+        import  pigeon
+        
         hist_candles = pigeon.HistoricalCandles(api_key='YOUR_API_KEY')
-        hist_candles.get_historical_candles(ticker='PETR4', lookback='5D', mode='absolute').plot(x='date', y='close_price', kind='scatter')
+        hist_candles.get_historical_candles(ticker='PETR4', period='5D', mode='relative').plot(x='date', y='close_price', kind='scatter')
         ```
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pigeonapi-python-client-0.10/pigeon/config.py` & `pigeonapi-python-client-0.9/pigeon/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 ### WebSocket 
 socket_urls = {
     'derivatives_realtime': {
         'trades': "wss://websockets.pigeonapi.io/v2/marketdata/trade/derivatives",
         'books': "wss://websockets.pigeonapi.io/v2/marketdata/book/derivatives",
     },
-    'derivatives_delayed': {
-        'trades': "wss://websockets.pigeonapi.io/v2/marketdata/trade/derivatives/delayed",
-    },
+    # 'derivatives_delayed': {
+    #     'trades': "wss://websockets.pigeonapi.io/v2/marketdata/trade/derivatives/delayed",
+    #     'books': "wss://websockets.pigeonapi.io/v2/marketdata/book/derivatives/delayed",
+    # },
     'stocks_realtime': {
         'trades': "wss://websockets.pigeonapi.io/v2/marketdata/trade/stocks",
         'books': "wss://websockets.pigeonapi.io/v2/marketdata/book/stocks",
     },
-    'stocks_delayed': {
-        'trades': "wss://websockets.pigeonapi.io/v2/marketdata/trade/stocks/delayed",
+    # 'stocks_delayed': {
+    #     'trades': "wss://websockets.pigeonapi.io/v2/marketdata/trade/stocks/delayed",
+    #     'books': "wss://websockets.pigeonapi.io/v2/marketdata/book/stocks/delayed",
+    # },
+    'options_realtime': {
+        'trades': "wss://websockets.pigeonapi.io/v2/marketdata/trade/options",
+        'books': "wss://websockets.pigeonapi.io/v2/marketdata/book/options",
     },
+    # 'options_delayed': {
+    #     'trades': "wss://websockets.pigeonapi.io/v2/marketdata/trade/options/delayed",
+    #     'books': "wss://websockets.pigeonapi.io/v2/marketdata/book/options/delayed",
+    # },
     'indices_realtime': "wss://websockets.pigeonapi.io/v2/marketdata/indices",
-    'indices_delayed': "wss://websockets.pigeonapi.io/v2/marketdata/indices/delayed"
+    # 'indices_delayed': "wss://websockets.pigeonapi.io/v2/marketdata/indices/delayed"
 }
 
 keys_socket = list(socket_urls.keys())
 
 valid_delayed_options = list(set([i.split('_')[1] for i in keys_socket]))
 valid_feeds = list(set([i.split('_')[0] for i in keys_socket]))
 
 def valid_ws_options(feed, target):
     return list(set(socket_urls[f'{feed}_{target}']))
 
 
 ### Rest
-
-url_apis = "https://dataservices.btgpactualsolutions.com/api/v2"
+url_apis = "https://gofast.btgpactualsolutions.com/api/v1.1/"
```

### Comparing `pigeonapi-python-client-0.10/pigeon/rest/authenticator.py` & `pigeonapi-python-client-0.9/pigeon/rest/authenticator.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class Authenticator:
     def __init__(self, api_key) -> None:
         self.api_key = api_key
         self._token = self.get_new_token()
 
     def get_new_token(self):
-        url = f"{url_apis}/authenticate"
+        url = f"{url_apis}authenticate"
         headersList = {
             "Content-Type": "application/json" 
         }
         payload = json.dumps({
             "api_key": self.api_key,
             "client_id": f"pigeon-client-python"
         })
```

### Comparing `pigeonapi-python-client-0.10/pigeon/rest/historical_candles.py` & `pigeonapi-python-client-0.9/pigeon/rest/intraday_candles.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,88 +1,85 @@
+
 from typing import Optional
 from ..exceptions import BadResponse
 import requests
 from ..config import url_apis
-from .authenticator import Authenticator
 import json
 import pandas as pd
+from .authenticator import Authenticator
 
-class HistoricalCandles:
+class IntradayCandles:
     """
-    This class provides historical candles for a given ticker or all tickers available for query.
+    This class provides realtime intraday candles for a given ticker or all tickers available for query.
 
     * Main use case:
 
-    >>> from pigeon import HistoricalCandles
-    >>> hist_candles = HistoricalCandles(
+    >>> from pigeon import IntradayCandles
+    >>> hist_candles = IntradayCandles(
     >>>     api_key='YOUR_API_KEY',
     >>> )
-    >>> hist_candles.get_historical_candles(
+    >>> obj.get_intraday_candles(
     >>>     ticker = 'PETR4',
-    >>>     lookback = '1M',
+    >>>     candle_period = '1m',
     >>>     mode = 'relative',
     >>>     raw_data = False
     >>> )
-    >>> hist_candles.get_available_tickers()
 
     Parameters
     ----------------
     api_key: str
         User identification key.
         Field is required.
     """
     def __init__(
         self,
-        api_key:Optional[str]
+        api_key: Optional[str]
     ):
         self.api_key = api_key
         self.token = Authenticator(self.api_key).token
         self.headers = {"authorization": f"authorization {self.token}"}
 
-    def get_historical_candles(
+    def get_intraday_candles(
         self,
         ticker:str,
-        lookback:str,
-        mode:str='absolute',
+        candle_period:str,
+        mode:str,
         raw_data:bool=False
-    ):
+    ):     
         """
-        This method provides historical candles for a given ticket in determined period.
+        This method provides realtime intraday candles for a given ticker.
 
         Parameters
         ----------------
         ticker: str
             Ticker that needs to be returned.
             Field is required. Example: 'PETR4'.
-        lookback: str
+        period: str
             Date period.
-            Field is required. Example: '5D', '1M', '6M', 'YTD', '1Y', '2Y' or '3Y'.
+            Field is required. Examples: '1m'.
         mode: str
             Candle mode.
-            Field is not required. Example: 'absolute' or 'relative'.
-            Default: 'absolute'.
+            Field is required. Example: 'absolute' or 'relative'.
         raw_data: bool
             If false, returns data in a dataframe. If true, returns raw data.
             Field is not required. Default: False.
-        """     
-        url = f"{url_apis}/marketdata/candles/historical?ticker={ticker}&lookback={lookback}&mode={mode}"
-
+        """
+        url = f"{url_apis}get_candles_intraday?ticker={ticker}&candle_period={candle_period}&mode={mode}"
         response = requests.request("GET", url,  headers=self.headers)
         if response.status_code == 200:
             response_data = json.loads(response.text)
             return response_data if raw_data else pd.DataFrame(response_data)
+        else:
+            response = json.loads(response.text)
+            raise BadResponse(f'Error: {response.get("ApiClientError")}.\n{response.get("SuggestedAction")}')
 
-        response = json.loads(response.text)
-        raise BadResponse(f'Error: {response.get("ApiClientError", "")}.\n{response.get("SuggestedAction", "")}')
-
-    def get_available_tickers(self):  
+    def get_available_tickers(self):
         """
         This method provides all tickers available for query.   
         """
-        url = f"{url_apis}/marketdata/candles/historical/available_tickers"
+        url = f"{url_apis}get_candles_intraday/available_tickers"
         response = requests.request("GET", url,  headers=self.headers)
-
         if response.status_code == 200:
             return json.loads(response.text).get('available_tickers', [])
         else:
             response = json.loads(response.text)
-            raise BadResponse(f'Error: {response.get("ApiClientError", "")}.\n{response.get("SuggestedAction", "")}')
+            raise BadResponse(f'Error: {response.get("ApiClientError")}.\n{response.get("SuggestedAction")}')
```

### Comparing `pigeonapi-python-client-0.10/pigeon/websocket/websocket_client.py` & `pigeonapi-python-client-0.9/pigeon/websocket/websocket_client.py`

 * *Files identical despite different names*

### Comparing `pigeonapi-python-client-0.10/pigeonapi_python_client.egg-info/PKG-INFO` & `pigeonapi-python-client-0.9/pigeonapi_python_client.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 Metadata-Version: 2.1
 Name: pigeonapi-python-client
-Version: 0.10
+Version: 0.9
 Summary: Python package containing several classes and data for extracting and manipulating market and trading data.
 Home-page: https://github.com/BTG-Pactual-Solutions/pigeonapi-python-client
 Author: PigeonAPI powered by BTG Pactual Solutions
 License: UNKNOWN
 Description: # Pigeon
         
         Pigeon is a Python library to get Brazilian Financial Market Data.
         
         ## Installation
         
         ```bash
         pip3 install pigeonapi-python-client
         ```
         
-        ## Example - WebSocket Books
-        ```python
-        import pigeon
-        ws = pigeon.WebSocketClient(api_key='YOUR_API_KEY', ws_type='books', instruments=['PETR4', 'VALE3'])
-        ws.run(on_message=lambda message: print(message))
-        ```
-        ## Example - WebSocket Trades Delayed
+        ## Example - WebSocket
+        
         ```python
         import pigeon
-        ws = pigeon.WebSocketClient(api_key='YOUR_API_KEY', ws_type='trades', target='delayed', instruments=['PETR4', 'VALE3'])
+        
+        ws = pigeon.WebSocketClient(api_key='YOUR_API_KEY', instruments=['PETR4', 'VALE3'])
         ws.run(on_message=lambda message: print(message))
         ```
-        
         ## Example - IntradayCandles
+        
         ```python
         import pigeon
+        
         int_candles = pigeon.IntradayCandles(api_key='YOUR_API_KEY')
-        int_candles.get_intraday_candles(market_type='stocks', tickers=['PETR4', 'VALE3'], candle_period='1m', mode='relative', raw_data=True)
+        int_candles.get_intraday_candles(ticker='PETR4', candle_period='1m', mode='relative')
         ```
-        ## Example - Plot HistoricalCandles
+        ## Example - HistoricalCandles
+        
         ```python
-        import pigeon
+        import  pigeon
+        
         hist_candles = pigeon.HistoricalCandles(api_key='YOUR_API_KEY')
-        hist_candles.get_historical_candles(ticker='PETR4', lookback='5D', mode='absolute').plot(x='date', y='close_price', kind='scatter')
+        hist_candles.get_historical_candles(ticker='PETR4', period='5D', mode='relative').plot(x='date', y='close_price', kind='scatter')
         ```
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pigeonapi-python-client-0.10/pigeonapi_python_client.egg-info/SOURCES.txt` & `pigeonapi-python-client-0.9/pigeonapi_python_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 setup.py
 pigeon/__init__.py
 pigeon/config.py
 pigeon/exceptions.py
 pigeon/rest/__init__.py
 pigeon/rest/authenticator.py
```

### Comparing `pigeonapi-python-client-0.10/setup.py` & `pigeonapi-python-client-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         with open(requirementPath) as f:
             install_requires = f.read().splitlines()
 
 description = "Python package containing several classes and data for extracting and manipulating market and trading data."
 
 setup(
     name='pigeonapi-python-client',
-    version='0.10',
+    version='0.9',
     description=description,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="PigeonAPI powered by BTG Pactual Solutions",
     packages=find_packages(),
     url="https://github.com/BTG-Pactual-Solutions/pigeonapi-python-client",
     install_requires=install_requires,
```

