# Comparing `tmp/vcsc_data_common-0.0.9.tar.gz` & `tmp/vcsc_data_common-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcsc_data_common-0.0.9.tar", last modified: Thu Mar 16 10:42:03 2023, max compression
+gzip compressed data, was "vcsc_data_common-0.1.0.tar", last modified: Tue Apr 18 03:33:56 2023, max compression
```

## Comparing `vcsc_data_common-0.0.9.tar` & `vcsc_data_common-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-03-16 10:42:03.027493 vcsc_data_common-0.0.9/
--rw-r--r--   0 pd         (501) staff       (20)      300 2023-03-16 10:42:03.027577 vcsc_data_common-0.0.9/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)      143 2023-02-22 09:16:04.000000 vcsc_data_common-0.0.9/README.md
--rw-r--r--   0 pd         (501) staff       (20)      673 2023-02-22 09:20:45.000000 vcsc_data_common-0.0.9/pyproject.toml
--rw-r--r--   0 pd         (501) staff       (20)      339 2023-03-16 10:42:03.027887 vcsc_data_common-0.0.9/setup.cfg
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-03-16 10:42:03.023209 vcsc_data_common-0.0.9/vcsc_data_common/
--rw-r--r--   0 pd         (501) staff       (20)      108 2023-02-22 09:07:01.000000 vcsc_data_common-0.0.9/vcsc_data_common/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-03-16 10:42:03.025569 vcsc_data_common-0.0.9/vcsc_data_common/ai_framework/
--rw-r--r--   0 pd         (501) staff       (20)       48 2023-02-22 09:02:01.000000 vcsc_data_common-0.0.9/vcsc_data_common/ai_framework/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     4520 2023-03-16 10:38:55.000000 vcsc_data_common-0.0.9/vcsc_data_common/ai_framework/interval_fetching.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-03-16 10:42:03.026027 vcsc_data_common-0.0.9/vcsc_data_common/live_price_data/
--rw-r--r--   0 pd         (501) staff       (20)     2181 2023-03-14 03:11:42.000000 vcsc_data_common-0.0.9/vcsc_data_common/live_price_data/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-03-16 10:42:03.026344 vcsc_data_common-0.0.9/vcsc_data_common/offline_price_data/
--rw-r--r--   0 pd         (501) staff       (20)      880 2023-03-14 02:58:59.000000 vcsc_data_common-0.0.9/vcsc_data_common/offline_price_data/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-03-16 10:42:03.026608 vcsc_data_common-0.0.9/vcsc_data_common/order/
--rw-r--r--   0 pd         (501) staff       (20)     1742 2023-03-14 03:08:00.000000 vcsc_data_common-0.0.9/vcsc_data_common/order/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-03-16 10:42:03.027206 vcsc_data_common-0.0.9/vcsc_data_common/portfolio_info/
--rw-r--r--   0 pd         (501) staff       (20)     2401 2023-03-07 02:02:42.000000 vcsc_data_common-0.0.9/vcsc_data_common/portfolio_info/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-03-16 10:42:03.024910 vcsc_data_common-0.0.9/vcsc_data_common.egg-info/
--rw-r--r--   0 pd         (501) staff       (20)      300 2023-03-16 10:42:03.000000 vcsc_data_common-0.0.9/vcsc_data_common.egg-info/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)      527 2023-03-16 10:42:03.000000 vcsc_data_common-0.0.9/vcsc_data_common.egg-info/SOURCES.txt
--rw-r--r--   0 pd         (501) staff       (20)        1 2023-03-16 10:42:03.000000 vcsc_data_common-0.0.9/vcsc_data_common.egg-info/dependency_links.txt
--rw-r--r--   0 pd         (501) staff       (20)       91 2023-03-16 10:42:03.000000 vcsc_data_common-0.0.9/vcsc_data_common.egg-info/requires.txt
--rw-r--r--   0 pd         (501) staff       (20)       17 2023-03-16 10:42:03.000000 vcsc_data_common-0.0.9/vcsc_data_common.egg-info/top_level.txt
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-18 03:33:56.687478 vcsc_data_common-0.1.0/
+-rw-r--r--   0 pd         (501) staff       (20)      300 2023-04-18 03:33:56.687570 vcsc_data_common-0.1.0/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)      143 2023-02-22 09:16:04.000000 vcsc_data_common-0.1.0/README.md
+-rw-r--r--   0 pd         (501) staff       (20)      799 2023-03-23 03:54:32.000000 vcsc_data_common-0.1.0/pyproject.toml
+-rw-r--r--   0 pd         (501) staff       (20)      339 2023-04-18 03:33:56.687895 vcsc_data_common-0.1.0/setup.cfg
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-18 03:33:56.683903 vcsc_data_common-0.1.0/vcsc_data_common/
+-rw-r--r--   0 pd         (501) staff       (20)      108 2023-02-22 09:07:01.000000 vcsc_data_common-0.1.0/vcsc_data_common/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-18 03:33:56.685319 vcsc_data_common-0.1.0/vcsc_data_common/ai_framework/
+-rw-r--r--   0 pd         (501) staff       (20)       48 2023-02-22 09:02:01.000000 vcsc_data_common-0.1.0/vcsc_data_common/ai_framework/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     4948 2023-03-31 09:44:29.000000 vcsc_data_common-0.1.0/vcsc_data_common/ai_framework/interval_fetching.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-18 03:33:56.685633 vcsc_data_common-0.1.0/vcsc_data_common/live_price_data/
+-rw-r--r--   0 pd         (501) staff       (20)     2338 2023-03-27 04:16:56.000000 vcsc_data_common-0.1.0/vcsc_data_common/live_price_data/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-18 03:33:56.686195 vcsc_data_common-0.1.0/vcsc_data_common/offline_price_data/
+-rw-r--r--   0 pd         (501) staff       (20)      880 2023-03-14 02:58:59.000000 vcsc_data_common-0.1.0/vcsc_data_common/offline_price_data/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-18 03:33:56.686879 vcsc_data_common-0.1.0/vcsc_data_common/order/
+-rw-r--r--   0 pd         (501) staff       (20)     3647 2023-03-27 04:29:07.000000 vcsc_data_common-0.1.0/vcsc_data_common/order/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-18 03:33:56.687236 vcsc_data_common-0.1.0/vcsc_data_common/portfolio_info/
+-rw-r--r--   0 pd         (501) staff       (20)     2658 2023-04-18 03:32:56.000000 vcsc_data_common-0.1.0/vcsc_data_common/portfolio_info/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-04-18 03:33:56.684874 vcsc_data_common-0.1.0/vcsc_data_common.egg-info/
+-rw-r--r--   0 pd         (501) staff       (20)      300 2023-04-18 03:33:56.000000 vcsc_data_common-0.1.0/vcsc_data_common.egg-info/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)      527 2023-04-18 03:33:56.000000 vcsc_data_common-0.1.0/vcsc_data_common.egg-info/SOURCES.txt
+-rw-r--r--   0 pd         (501) staff       (20)        1 2023-04-18 03:33:56.000000 vcsc_data_common-0.1.0/vcsc_data_common.egg-info/dependency_links.txt
+-rw-r--r--   0 pd         (501) staff       (20)      140 2023-04-18 03:33:56.000000 vcsc_data_common-0.1.0/vcsc_data_common.egg-info/requires.txt
+-rw-r--r--   0 pd         (501) staff       (20)       17 2023-04-18 03:33:56.000000 vcsc_data_common-0.1.0/vcsc_data_common.egg-info/top_level.txt
```

### Comparing `vcsc_data_common-0.0.9/vcsc_data_common/ai_framework/interval_fetching.py` & `vcsc_data_common-0.1.0/vcsc_data_common/ai_framework/interval_fetching.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,43 @@
+from dataclasses import dataclass
 from vcsc_data_common.live_price_data import DataFetcher as LiveDataFetcher, MarketStatus
 from vcsc_data_common.offline_price_data import DataFetcher as OfflineDataFetcher
 import pandas as pd
 import time
 import logging
 import threading
 
 
+@dataclass
+class FetchingTimeFrameConfig:
+    time_frame: str
+    is_fill_gap: bool = False
+
+
 class IntervalFetching:
     offline_data_dfs: list[pd.DataFrame] = []
     live_data_dfs: list[pd.DataFrame] = []
     is_new_live_data: bool
 
-    def __init__(self, aws_access_key: str, aws_secret_key: str, time_frames: list[str], interval: int, callback: callable, is_fill_gap: bool = False) -> None:
+    def __init__(self, aws_access_key: str, aws_secret_key: str, fetching_time_frame_configs: list[FetchingTimeFrameConfig], interval: int, callback: callable) -> None:
         self.aws_access_key = aws_access_key
         self.aws_secret_key = aws_secret_key
-        self.time_frames = time_frames
+        self.fetching_time_frame_configs = fetching_time_frame_configs
         self.callback = callback
         self.interval = interval
         self.live_modification_time = None
-        self.is_fill_gap = is_fill_gap
         self.live_data_fetchers: list[LiveDataFetcher] = []
         self.offline_data_fetchers: list[OfflineDataFetcher] = []
 
-        for time_frame in time_frames:
+        for fetching_time_frame_config in fetching_time_frame_configs:
 
             live_data_fetcher = LiveDataFetcher(
-                aws_access_key, aws_secret_key, time_frame, is_fill_gap)
+                aws_access_key, aws_secret_key, fetching_time_frame_config.time_frame, fetching_time_frame_config.is_fill_gap)
             offline_data_fetcher = OfflineDataFetcher(
-                aws_access_key, aws_secret_key, time_frame, is_fill_gap)
+                aws_access_key, aws_secret_key, fetching_time_frame_config.time_frame, fetching_time_frame_config.is_fill_gap)
 
             self.live_data_fetchers.append(live_data_fetcher)
             self.offline_data_fetchers.append(offline_data_fetcher)
 
             self.offline_data_dfs.append(pd.DataFrame())
             self.live_data_dfs.append(pd.DataFrame())
 
@@ -43,22 +49,26 @@
             self.fetch_all_live_data()
 
             if(self.is_new_live_data):
 
                 # union all df & return
                 data_arr: list[pd.DataFrame] = []
 
-                for index, time_frame in enumerate(self.time_frames):
+                for index in range(self.fetching_time_frame_configs.__len__()):
                     offline_data_df = self.offline_data_dfs[index]
                     live_data_df = self.live_data_dfs[index]
                     union_df = pd.concat([offline_data_df, live_data_df])
 
                     data_arr.append(union_df)
 
-                self.callback(*data_arr, self.live_modification_time)
+                market_status_df = self.live_data_fetchers[0].get_market_status(
+                )
+
+                self.callback(*data_arr, market_status_df,
+                              self.live_modification_time)
 
             else:
                 logging.debug('data has no change')
 
             self.is_new_live_data = False
             time.sleep(self.interval)
```

### Comparing `vcsc_data_common-0.0.9/vcsc_data_common/live_price_data/__init__.py` & `vcsc_data_common-0.1.0/vcsc_data_common/live_price_data/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import logging
 from deltalake import DeltaTable
 import pandas as pd
 import requests
 from enum import Enum
 
 
 class MarketStatus(Enum):
@@ -49,16 +50,23 @@
         })
 
         actions_df = dt.get_add_actions().to_pandas()
         self.last_modification_time = actions_df.iloc[0]['modification_time']
         return self.last_modification_time
 
     def get_market_status(self) -> pd.DataFrame:
+
         response = requests.get(
             'https://mt.vcsc.com.vn/api/price/marketStatus/getAll')
-        json_data = json.loads(response.text)
-        arr = []
-        for key in json_data:
-            arr.append(
-                {'marketCode': json_data[key]['marketCode'], 'status': json_data[key]['status']})
+        try:
+
+            json_data = json.loads(response.text)
+            arr = []
+            for key in json_data:
+                arr.append(
+                    {'marketCode': json_data[key]['marketCode'], 'status': json_data[key]['status']})
+
+        except Exception as e:
+            logging.error(f'response {response.text}')
+            raise e
 
         return pd.DataFrame(arr)
```

### Comparing `vcsc_data_common-0.0.9/vcsc_data_common/offline_price_data/__init__.py` & `vcsc_data_common-0.1.0/vcsc_data_common/offline_price_data/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.0.9/vcsc_data_common/portfolio_info/__init__.py` & `vcsc_data_common-0.1.0/vcsc_data_common/portfolio_info/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,53 @@
+import json
+import logging
+import requests
 from sqlalchemy import create_engine
 import pandas as pd
 
 
 class PortfolioInfo:
     def __init__(self, paper_trading_db_host: str, paper_trading_db_port: int, paper_trading_db_username: str,
-                 paper_trading_db_password: str, paper_trading_db_name: str):
+                 paper_trading_db_password: str, paper_trading_db_name: str, paper_trading_api_end_point: str):
         self.paper_trading_db_host = paper_trading_db_host
         self.paper_trading_db_port = paper_trading_db_port
         self.paper_trading_db_username = paper_trading_db_username
         self.paper_trading_db_password = paper_trading_db_password
         self.paper_trading_db_name = paper_trading_db_name
+        self.paper_trading_api_end_point = paper_trading_api_end_point
 
         paper_trading_db_connection_str = f'postgresql://{paper_trading_db_username}:{paper_trading_db_password}@{paper_trading_db_host}:{paper_trading_db_port}/{paper_trading_db_name}'
         self.paper_trading_db_connection = create_engine(
             paper_trading_db_connection_str).connect()
 
     def get_all_portfolio(self):
-        return pd.read_sql(f"""  
-
-            with stock_portfolio as (
-                select t3.id as "portfolioId",t1.username,t1.symbol,COALESCE("latestMatchPrice",0) as "latestMatchPrice","totalAmount","availableAmount", "averageMatchedPrice","targetPercent"
+        return pd.read_sql(f""" 
+            select t1."portfolioConfigId",t4."tradingModel",t4."portfolioModel",t1.username,t1.symbol,COALESCE("latestMatchPrice",0) as "latestMatchPrice",
+                "totalAmount",CASE WHEN "forceSellAmount" > "availableAmount" THEN 0 ELSE "availableAmount" - "forceSellAmount"  END as "availableAmount",
+                "pendingAmount","scheduledAmount", "averageMatchedPrice","targetPercent",
+                "balance","initBalance", t1."cutoffDate", t1."startDate",t1."endDate", "forceSellAmount" , t1."portfolioType"
                 from "portfolio" t1
                 left join "symbol_info" t2 on t1.symbol = t2.symbol
-                left join "cash" t3 on t1.username = t3.username
-                WHERE t1.symbol != 'CASH'
-            )
-            , cash_portfolio as (
-                select t1."id" as "portfolioId",t1.username,'CASH' as symbol, 0::double precision as "latestMatchPrice",
-                "currentCash" + "blockedCash" as "totalAmount", "currentCash" + "blockedCash" as "availableAmount",
-                0::double precision as "averageMatchedPrice",t2."targetPercent"
-                from "cash" t1 
-                left join 
-                (SELECT * FROM "portfolio" WHERE symbol = 'CASH') t2 on t1.username = t2.username
-            )
-
-            select * from stock_portfolio 
-            union all
-            select * from cash_portfolio
-
+                left join "portfolio_config" t4 on t1."portfolioConfigId" = t4.id
         """, con=self.paper_trading_db_connection)
 
-    def update_target_percent_portfolio(self, portfolio_data: dict):
+    def update_target_percent_portfolio(self, portfolio_data: dict, cycle_length: int, portfolioModel: int):
 
-        for key in portfolio_data:
-            target_percent = portfolio_data[key]
+        url = f"{self.paper_trading_api_end_point}/portfolioRatio/updateNewRatio"
 
-            self.paper_trading_db_connection.execute(
-                f""" UPDATE portfolio set "targetPercent" = {target_percent}  WHERE symbol = '{key}' """)
+        payload = json.dumps({
+            "ratio": portfolio_data,
+            "portfolioModel": portfolioModel
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+
+        response = requests.request("POST", url, headers=headers, data=payload)
+
+        if(response.status_code == 200):
+            logging.info(
+                f'update_target_percent_portfolio ==> {response.text}')
+        else:
+            logging.error(
+                f'update_target_percent_portfolio ==> {response.text}')
+            raise Exception('update_target_percent_portfolio failed')
```

### Comparing `vcsc_data_common-0.0.9/vcsc_data_common.egg-info/SOURCES.txt` & `vcsc_data_common-0.1.0/vcsc_data_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

