# Comparing `tmp/vcsc_data_common-0.1.0.tar.gz` & `tmp/vcsc_data_common-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcsc_data_common-0.1.0.tar", last modified: Tue Apr 18 03:33:56 2023, max compression
+gzip compressed data, was "vcsc_data_common-0.1.1.tar", last modified: Tue Apr 18 08:33:11 2023, max compression
```

## Comparing `vcsc_data_common-0.1.0.tar` & `vcsc_data_common-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-18 03:33:56.687478 vcsc_data_common-0.1.0/
--rw-r--r--   0 pd         (501) staff       (20)      300 2023-04-18 03:33:56.687570 vcsc_data_common-0.1.0/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)      143 2023-02-22 09:16:04.000000 vcsc_data_common-0.1.0/README.md
--rw-r--r--   0 pd         (501) staff       (20)      799 2023-03-23 03:54:32.000000 vcsc_data_common-0.1.0/pyproject.toml
--rw-r--r--   0 pd         (501) staff       (20)      339 2023-04-18 03:33:56.687895 vcsc_data_common-0.1.0/setup.cfg
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-18 03:33:56.683903 vcsc_data_common-0.1.0/vcsc_data_common/
--rw-r--r--   0 pd         (501) staff       (20)      108 2023-02-22 09:07:01.000000 vcsc_data_common-0.1.0/vcsc_data_common/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-18 03:33:56.685319 vcsc_data_common-0.1.0/vcsc_data_common/ai_framework/
--rw-r--r--   0 pd         (501) staff       (20)       48 2023-02-22 09:02:01.000000 vcsc_data_common-0.1.0/vcsc_data_common/ai_framework/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     4948 2023-03-31 09:44:29.000000 vcsc_data_common-0.1.0/vcsc_data_common/ai_framework/interval_fetching.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-18 03:33:56.685633 vcsc_data_common-0.1.0/vcsc_data_common/live_price_data/
--rw-r--r--   0 pd         (501) staff       (20)     2338 2023-03-27 04:16:56.000000 vcsc_data_common-0.1.0/vcsc_data_common/live_price_data/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-18 03:33:56.686195 vcsc_data_common-0.1.0/vcsc_data_common/offline_price_data/
--rw-r--r--   0 pd         (501) staff       (20)      880 2023-03-14 02:58:59.000000 vcsc_data_common-0.1.0/vcsc_data_common/offline_price_data/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-18 03:33:56.686879 vcsc_data_common-0.1.0/vcsc_data_common/order/
--rw-r--r--   0 pd         (501) staff       (20)     3647 2023-03-27 04:29:07.000000 vcsc_data_common-0.1.0/vcsc_data_common/order/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-18 03:33:56.687236 vcsc_data_common-0.1.0/vcsc_data_common/portfolio_info/
--rw-r--r--   0 pd         (501) staff       (20)     2658 2023-04-18 03:32:56.000000 vcsc_data_common-0.1.0/vcsc_data_common/portfolio_info/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-18 03:33:56.684874 vcsc_data_common-0.1.0/vcsc_data_common.egg-info/
--rw-r--r--   0 pd         (501) staff       (20)      300 2023-04-18 03:33:56.000000 vcsc_data_common-0.1.0/vcsc_data_common.egg-info/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)      527 2023-04-18 03:33:56.000000 vcsc_data_common-0.1.0/vcsc_data_common.egg-info/SOURCES.txt
--rw-r--r--   0 pd         (501) staff       (20)        1 2023-04-18 03:33:56.000000 vcsc_data_common-0.1.0/vcsc_data_common.egg-info/dependency_links.txt
--rw-r--r--   0 pd         (501) staff       (20)      140 2023-04-18 03:33:56.000000 vcsc_data_common-0.1.0/vcsc_data_common.egg-info/requires.txt
--rw-r--r--   0 pd         (501) staff       (20)       17 2023-04-18 03:33:56.000000 vcsc_data_common-0.1.0/vcsc_data_common.egg-info/top_level.txt
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-18 08:33:11.552975 vcsc_data_common-0.1.1/
+-rw-r--r--   0 pd         (501) staff       (20)      300 2023-04-18 08:33:11.553065 vcsc_data_common-0.1.1/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)      143 2023-02-22 09:16:04.000000 vcsc_data_common-0.1.1/README.md
+-rw-r--r--   0 pd         (501) staff       (20)      799 2023-03-23 03:54:32.000000 vcsc_data_common-0.1.1/pyproject.toml
+-rw-r--r--   0 pd         (501) staff       (20)      339 2023-04-18 08:33:11.553403 vcsc_data_common-0.1.1/setup.cfg
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-18 08:33:11.550146 vcsc_data_common-0.1.1/vcsc_data_common/
+-rw-r--r--   0 pd         (501) staff       (20)      108 2023-02-22 09:07:01.000000 vcsc_data_common-0.1.1/vcsc_data_common/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-18 08:33:11.551518 vcsc_data_common-0.1.1/vcsc_data_common/ai_framework/
+-rw-r--r--   0 pd         (501) staff       (20)       48 2023-02-22 09:02:01.000000 vcsc_data_common-0.1.1/vcsc_data_common/ai_framework/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     4948 2023-03-31 09:44:29.000000 vcsc_data_common-0.1.1/vcsc_data_common/ai_framework/interval_fetching.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-18 08:33:11.551835 vcsc_data_common-0.1.1/vcsc_data_common/live_price_data/
+-rw-r--r--   0 pd         (501) staff       (20)     2338 2023-03-27 04:16:56.000000 vcsc_data_common-0.1.1/vcsc_data_common/live_price_data/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-18 08:33:11.552120 vcsc_data_common-0.1.1/vcsc_data_common/offline_price_data/
+-rw-r--r--   0 pd         (501) staff       (20)      880 2023-03-14 02:58:59.000000 vcsc_data_common-0.1.1/vcsc_data_common/offline_price_data/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-18 08:33:11.552393 vcsc_data_common-0.1.1/vcsc_data_common/order/
+-rw-r--r--   0 pd         (501) staff       (20)     3647 2023-03-27 04:29:07.000000 vcsc_data_common-0.1.1/vcsc_data_common/order/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-18 08:33:11.552715 vcsc_data_common-0.1.1/vcsc_data_common/portfolio_info/
+-rw-r--r--   0 pd         (501) staff       (20)     3586 2023-04-18 08:32:03.000000 vcsc_data_common-0.1.1/vcsc_data_common/portfolio_info/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-18 08:33:11.550903 vcsc_data_common-0.1.1/vcsc_data_common.egg-info/
+-rw-r--r--   0 pd         (501) staff       (20)      300 2023-04-18 08:33:11.000000 vcsc_data_common-0.1.1/vcsc_data_common.egg-info/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)      527 2023-04-18 08:33:11.000000 vcsc_data_common-0.1.1/vcsc_data_common.egg-info/SOURCES.txt
+-rw-r--r--   0 pd         (501) staff       (20)        1 2023-04-18 08:33:11.000000 vcsc_data_common-0.1.1/vcsc_data_common.egg-info/dependency_links.txt
+-rw-r--r--   0 pd         (501) staff       (20)      140 2023-04-18 08:33:11.000000 vcsc_data_common-0.1.1/vcsc_data_common.egg-info/requires.txt
+-rw-r--r--   0 pd         (501) staff       (20)       17 2023-04-18 08:33:11.000000 vcsc_data_common-0.1.1/vcsc_data_common.egg-info/top_level.txt
```

### Comparing `vcsc_data_common-0.1.0/pyproject.toml` & `vcsc_data_common-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.0/vcsc_data_common/ai_framework/interval_fetching.py` & `vcsc_data_common-0.1.1/vcsc_data_common/ai_framework/interval_fetching.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.0/vcsc_data_common/live_price_data/__init__.py` & `vcsc_data_common-0.1.1/vcsc_data_common/live_price_data/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.0/vcsc_data_common/offline_price_data/__init__.py` & `vcsc_data_common-0.1.1/vcsc_data_common/offline_price_data/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.0/vcsc_data_common/order/__init__.py` & `vcsc_data_common-0.1.1/vcsc_data_common/order/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.0/vcsc_data_common/portfolio_info/__init__.py` & `vcsc_data_common-0.1.1/vcsc_data_common/portfolio_info/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 import requests
 from sqlalchemy import create_engine
 import pandas as pd
 
 
 class PortfolioInfo:
     def __init__(self, paper_trading_db_host: str, paper_trading_db_port: int, paper_trading_db_username: str,
-                 paper_trading_db_password: str, paper_trading_db_name: str, paper_trading_api_end_point: str):
+                 paper_trading_db_password: str, paper_trading_db_name: str, paper_trading_api_end_point: str, ai_portfolio_service_host: str):
         self.paper_trading_db_host = paper_trading_db_host
         self.paper_trading_db_port = paper_trading_db_port
         self.paper_trading_db_username = paper_trading_db_username
         self.paper_trading_db_password = paper_trading_db_password
         self.paper_trading_db_name = paper_trading_db_name
         self.paper_trading_api_end_point = paper_trading_api_end_point
+        self.ai_portfolio_service_host = ai_portfolio_service_host
 
         paper_trading_db_connection_str = f'postgresql://{paper_trading_db_username}:{paper_trading_db_password}@{paper_trading_db_host}:{paper_trading_db_port}/{paper_trading_db_name}'
         self.paper_trading_db_connection = create_engine(
             paper_trading_db_connection_str).connect()
 
     def get_all_portfolio(self):
         return pd.read_sql(f""" 
@@ -28,14 +29,15 @@
                 from "portfolio" t1
                 left join "symbol_info" t2 on t1.symbol = t2.symbol
                 left join "portfolio_config" t4 on t1."portfolioConfigId" = t4.id
         """, con=self.paper_trading_db_connection)
 
     def update_target_percent_portfolio(self, portfolio_data: dict, cycle_length: int, portfolioModel: int):
 
+        ######  update ratio mới cho backtest  #######
         url = f"{self.paper_trading_api_end_point}/portfolioRatio/updateNewRatio"
 
         payload = json.dumps({
             "ratio": portfolio_data,
             "portfolioModel": portfolioModel
         })
         headers = {
@@ -47,7 +49,29 @@
         if(response.status_code == 200):
             logging.info(
                 f'update_target_percent_portfolio ==> {response.text}')
         else:
             logging.error(
                 f'update_target_percent_portfolio ==> {response.text}')
             raise Exception('update_target_percent_portfolio failed')
+
+        ######  update ratio mới cho ai_portfolio_service  #######
+        url = f"{self.ai_portfolio_service_host}/portfolio/update"
+
+        payload = json.dumps({
+            "ratio": portfolio_data,
+            "portfolioModel": portfolioModel,
+            "cycleLength": cycle_length
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+
+        response = requests.request("POST", url, headers=headers, data=payload)
+
+        if(response.status_code == 200):
+            logging.info(
+                f'update ai_portfolio_service ==> {response.text}')
+        else:
+            logging.error(
+                f'update ai_portfolio_service ==> {response.text}')
+            raise Exception('update ai_portfolio_service failed')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `vcsc_data_common-0.1.0/vcsc_data_common.egg-info/SOURCES.txt` & `vcsc_data_common-0.1.1/vcsc_data_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

