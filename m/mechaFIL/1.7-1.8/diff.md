# Comparing `tmp/mechaFIL-1.7.tar.gz` & `tmp/mechaFIL-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mechaFIL-1.7.tar", last modified: Tue Feb 28 15:40:11 2023, max compression
+gzip compressed data, was "mechaFIL-1.8.tar", last modified: Tue Apr 18 13:38:50 2023, max compression
```

## Comparing `mechaFIL-1.7.tar` & `mechaFIL-1.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 maria      (501) staff       (20)        0 2023-02-28 15:40:11.646216 mechaFIL-1.7/
--rw-r--r--   0 maria      (501) staff       (20)     1069 2022-07-18 12:27:46.000000 mechaFIL-1.7/LICENSE
--rw-r--r--   0 maria      (501) staff       (20)     6390 2023-02-28 15:40:11.646074 mechaFIL-1.7/PKG-INFO
--rw-r--r--   0 maria      (501) staff       (20)     5747 2023-02-28 15:39:50.000000 mechaFIL-1.7/README.md
-drwxr-xr-x   0 maria      (501) staff       (20)        0 2023-02-28 15:40:11.643429 mechaFIL-1.7/mechaFIL.egg-info/
--rw-r--r--   0 maria      (501) staff       (20)     6390 2023-02-28 15:40:11.000000 mechaFIL-1.7/mechaFIL.egg-info/PKG-INFO
--rw-r--r--   0 maria      (501) staff       (20)      409 2023-02-28 15:40:11.000000 mechaFIL-1.7/mechaFIL.egg-info/SOURCES.txt
--rw-r--r--   0 maria      (501) staff       (20)        1 2023-02-28 15:40:11.000000 mechaFIL-1.7/mechaFIL.egg-info/dependency_links.txt
--rw-r--r--   0 maria      (501) staff       (20)       39 2023-02-28 15:40:11.000000 mechaFIL-1.7/mechaFIL.egg-info/requires.txt
--rw-r--r--   0 maria      (501) staff       (20)        9 2023-02-28 15:40:11.000000 mechaFIL-1.7/mechaFIL.egg-info/top_level.txt
-drwxr-xr-x   0 maria      (501) staff       (20)        0 2023-02-28 15:40:11.645762 mechaFIL-1.7/mechafil/
--rw-r--r--   0 maria      (501) staff       (20)      316 2023-02-28 15:39:50.000000 mechaFIL-1.7/mechafil/__init__.py
--rw-r--r--   0 maria      (501) staff       (20)     9008 2023-02-28 09:25:10.000000 mechaFIL-1.7/mechafil/data.py
--rw-r--r--   0 maria      (501) staff       (20)    13496 2023-02-28 09:25:10.000000 mechaFIL-1.7/mechafil/data_spacescope.py
--rw-r--r--   0 maria      (501) staff       (20)     8476 2023-02-23 08:36:22.000000 mechaFIL-1.7/mechafil/data_starboard.py
--rw-r--r--   0 maria      (501) staff       (20)     4547 2023-01-13 10:01:02.000000 mechaFIL-1.7/mechafil/locking.py
--rw-r--r--   0 maria      (501) staff       (20)     3876 2023-01-13 10:01:02.000000 mechaFIL-1.7/mechafil/minting.py
--rw-r--r--   0 maria      (501) staff       (20)    11608 2023-01-13 10:01:02.000000 mechaFIL-1.7/mechafil/power.py
--rw-r--r--   0 maria      (501) staff       (20)     4013 2023-02-28 09:25:10.000000 mechaFIL-1.7/mechafil/sim.py
--rw-r--r--   0 maria      (501) staff       (20)     6963 2023-01-13 10:01:02.000000 mechaFIL-1.7/mechafil/supply.py
--rw-r--r--   0 maria      (501) staff       (20)      207 2023-01-13 10:01:02.000000 mechaFIL-1.7/mechafil/utils.py
--rw-r--r--   0 maria      (501) staff       (20)     3013 2022-12-03 11:19:59.000000 mechaFIL-1.7/mechafil/vesting.py
--rw-r--r--   0 maria      (501) staff       (20)       38 2023-02-28 15:40:11.646259 mechaFIL-1.7/setup.cfg
--rw-r--r--   0 maria      (501) staff       (20)      905 2023-02-28 15:39:50.000000 mechaFIL-1.7/setup.py
+drwxr-xr-x   0 kiran      (501) staff       (20)        0 2023-04-18 13:38:50.831648 mechaFIL-1.8/
+-rw-r--r--   0 kiran      (501) staff       (20)     1069 2022-11-03 16:37:39.000000 mechaFIL-1.8/LICENSE
+-rw-r--r--   0 kiran      (501) staff       (20)     6353 2023-04-18 13:38:50.831502 mechaFIL-1.8/PKG-INFO
+-rw-r--r--   0 kiran      (501) staff       (20)     5747 2023-04-18 13:30:28.000000 mechaFIL-1.8/README.md
+drwxr-xr-x   0 kiran      (501) staff       (20)        0 2023-04-18 13:38:50.829161 mechaFIL-1.8/mechaFIL.egg-info/
+-rw-r--r--   0 kiran      (501) staff       (20)     6353 2023-04-18 13:38:50.000000 mechaFIL-1.8/mechaFIL.egg-info/PKG-INFO
+-rw-r--r--   0 kiran      (501) staff       (20)      409 2023-04-18 13:38:50.000000 mechaFIL-1.8/mechaFIL.egg-info/SOURCES.txt
+-rw-r--r--   0 kiran      (501) staff       (20)        1 2023-04-18 13:38:50.000000 mechaFIL-1.8/mechaFIL.egg-info/dependency_links.txt
+-rw-r--r--   0 kiran      (501) staff       (20)       39 2023-04-18 13:38:50.000000 mechaFIL-1.8/mechaFIL.egg-info/requires.txt
+-rw-r--r--   0 kiran      (501) staff       (20)        9 2023-04-18 13:38:50.000000 mechaFIL-1.8/mechaFIL.egg-info/top_level.txt
+drwxr-xr-x   0 kiran      (501) staff       (20)        0 2023-04-18 13:38:50.831213 mechaFIL-1.8/mechafil/
+-rw-r--r--   0 kiran      (501) staff       (20)      316 2023-04-18 13:30:28.000000 mechaFIL-1.8/mechafil/__init__.py
+-rw-r--r--   0 kiran      (501) staff       (20)     9057 2023-04-18 13:30:31.000000 mechaFIL-1.8/mechafil/data.py
+-rw-r--r--   0 kiran      (501) staff       (20)    13562 2023-04-18 13:30:31.000000 mechaFIL-1.8/mechafil/data_spacescope.py
+-rw-r--r--   0 kiran      (501) staff       (20)     8476 2023-04-18 13:30:28.000000 mechaFIL-1.8/mechafil/data_starboard.py
+-rw-r--r--   0 kiran      (501) staff       (20)     4547 2023-04-18 13:30:28.000000 mechaFIL-1.8/mechafil/locking.py
+-rw-r--r--   0 kiran      (501) staff       (20)     3876 2022-12-21 17:17:26.000000 mechaFIL-1.8/mechafil/minting.py
+-rw-r--r--   0 kiran      (501) staff       (20)    11608 2023-04-18 13:30:28.000000 mechaFIL-1.8/mechafil/power.py
+-rw-r--r--   0 kiran      (501) staff       (20)     4264 2023-04-18 13:30:31.000000 mechaFIL-1.8/mechafil/sim.py
+-rw-r--r--   0 kiran      (501) staff       (20)     6974 2023-04-18 13:30:31.000000 mechaFIL-1.8/mechafil/supply.py
+-rw-r--r--   0 kiran      (501) staff       (20)      207 2023-04-18 13:30:28.000000 mechaFIL-1.8/mechafil/utils.py
+-rw-r--r--   0 kiran      (501) staff       (20)     3013 2022-12-05 15:42:18.000000 mechaFIL-1.8/mechafil/vesting.py
+-rw-r--r--   0 kiran      (501) staff       (20)       38 2023-04-18 13:38:50.831683 mechaFIL-1.8/setup.cfg
+-rw-r--r--   0 kiran      (501) staff       (20)      905 2023-04-18 13:30:31.000000 mechaFIL-1.8/setup.py
```

### Comparing `mechaFIL-1.7/LICENSE` & `mechaFIL-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mechaFIL-1.7/PKG-INFO` & `mechaFIL-1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: mechaFIL
-Version: 1.7
+Version: 1.8
 Summary: Mechanistic model for the Filecoin Economy
 Author: Maria Silva, Tom Mellan, Kiran Karra
 Author-email: misilva73@gmail.com, t.mellan@imperial.ac.uk, kiran.karra@gmail.com
-License: UNKNOWN
 Project-URL: Documentation, https://github.com/protocol/filecoin-mecha-twin
 Project-URL: Source, https://github.com/protocol/filecoin-mecha-twin
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -133,9 +131,7 @@
 mecha_data.setup_spacecope(path_to_auth_cfg)
 ```
 
 ## References
 
 * [Power model spec](https://hackmd.io/@cryptoecon/SkapZkrdc)
 * [Locking model spec](https://hackmd.io/@cryptoecon/SJv_CGvY9)
-
-
```

### Comparing `mechaFIL-1.7/README.md` & `mechaFIL-1.8/README.md`

 * *Files identical despite different names*

### Comparing `mechaFIL-1.7/mechaFIL.egg-info/PKG-INFO` & `mechaFIL-1.8/mechaFIL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: mechaFIL
-Version: 1.7
+Version: 1.8
 Summary: Mechanistic model for the Filecoin Economy
 Author: Maria Silva, Tom Mellan, Kiran Karra
 Author-email: misilva73@gmail.com, t.mellan@imperial.ac.uk, kiran.karra@gmail.com
-License: UNKNOWN
 Project-URL: Documentation, https://github.com/protocol/filecoin-mecha-twin
 Project-URL: Source, https://github.com/protocol/filecoin-mecha-twin
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -133,9 +131,7 @@
 mecha_data.setup_spacecope(path_to_auth_cfg)
 ```
 
 ## References
 
 * [Power model spec](https://hackmd.io/@cryptoecon/SkapZkrdc)
 * [Locking model spec](https://hackmd.io/@cryptoecon/SJv_CGvY9)
-
-
```

### Comparing `mechaFIL-1.7/mechafil/data.py` & `mechaFIL-1.8/mechafil/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import pandas as pd
 import numpy as np
 import datetime
 from typing import Tuple
 
-from . import data_spacescope, data_starboard
 DEFAULT_DATA_BACKEND = 'spacescope'
+NETWORK_START = datetime.datetime(2020, 10, 15)
+
+from . import data_spacescope, data_starboard
 
 spacescope_obj = None
 def setup_spacescope(auth_config_or_token):
     global spacescope_obj
     spacescope_obj = data_spacescope.SpacescopeDataConnection(auth_config_or_token)
 
 def check_if_spacescope_configured():
```

### Comparing `mechaFIL-1.7/mechafil/data_spacescope.py` & `mechaFIL-1.8/mechafil/data_spacescope.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 from typing import Tuple, List
 import os
 import json
 
 EXBI = 2**60
 PIB = 2**50
 
-NETWORK_START = datetime.datetime(2020, 10, 15)
 DEFAULT_SPACESCOPE_CHUNK_SIZE_IN_DAYS = 90
 DEFAULT_AUTH_CONFIG = os.path.join(os.path.dirname(__file__), 'cfg', 'spacescope_auth.json')
 
+from .data import NETWORK_START
+
 class SpacescopeDataConnection:
     auth_token = ""
 
     def __init__(self, auth_config_or_token: str):
         if os.path.isfile(auth_config_or_token):
             # assume it is a JSON config file with key: auth_key
             try:
@@ -255,15 +256,15 @@
     @staticmethod
     def query_historical_baseline_power(start_date: datetime.date = None,
                                 end_date: datetime.date = None,
                                 chunk_days: int = DEFAULT_SPACESCOPE_CHUNK_SIZE_IN_DAYS) -> pd.DataFrame:
         if start_date is None:
             start_date = NETWORK_START
         if end_date is None:
-            end_date = datetime.datetime.today()
+            end_date = datetime.datetime.today()-datetime.timedelta(days=2)
 
         historical_power_df = SpacescopeDataConnection.query_historical_power(
             start_date, end_date, chunk_days=chunk_days
         )
 
         bp_df = historical_power_df[['date', 'baseline_power']]
         bp_df = bp_df.rename(columns={'baseline_power': 'baseline'})
@@ -272,15 +273,15 @@
     @staticmethod
     def query_historical_rb_power(start_date: datetime.date = None,
                                 end_date: datetime.date = None,
                                 chunk_days: int = DEFAULT_SPACESCOPE_CHUNK_SIZE_IN_DAYS) -> pd.DataFrame:
         if start_date is None:
             start_date = NETWORK_START
         if end_date is None:
-            end_date = datetime.datetime.today()
+            end_date = datetime.datetime.today()-datetime.timedelta(days=2)
 
         historical_power_df = SpacescopeDataConnection.query_historical_power(
             start_date, end_date, chunk_days=chunk_days
         )
 
         rbp_df = historical_power_df[['date', 'total_raw_bytes_power']]
         rbp_df = rbp_df.rename(columns={'total_raw_bytes_power': 'rb_power'})
@@ -289,15 +290,15 @@
     @staticmethod
     def query_historical_qa_power(start_date: datetime.date = None,
                                 end_date: datetime.date = None,
                                 chunk_days: int = DEFAULT_SPACESCOPE_CHUNK_SIZE_IN_DAYS) -> pd.DataFrame:
         if start_date is None:
             start_date = NETWORK_START
         if end_date is None:
-            end_date = datetime.datetime.today()
+            end_date = datetime.datetime.today()-datetime.timedelta(days=2)
 
         historical_power_df = SpacescopeDataConnection.query_historical_power(
             start_date, end_date, chunk_days=chunk_days
         )
         qap_df = historical_power_df[['date', 'total_raw_bytes_power']]
         qap_df = qap_df.rename(columns={'total_qa_bytes_power': 'qa_power'})
```

### Comparing `mechaFIL-1.7/mechafil/data_starboard.py` & `mechaFIL-1.8/mechafil/data_starboard.py`

 * *Files identical despite different names*

### Comparing `mechaFIL-1.7/mechafil/locking.py` & `mechaFIL-1.8/mechafil/locking.py`

 * *Files identical despite different names*

### Comparing `mechaFIL-1.7/mechafil/minting.py` & `mechaFIL-1.8/mechafil/minting.py`

 * *Files identical despite different names*

### Comparing `mechaFIL-1.7/mechafil/power.py` & `mechaFIL-1.8/mechafil/power.py`

 * *Files identical despite different names*

### Comparing `mechaFIL-1.7/mechafil/sim.py` & `mechaFIL-1.8/mechafil/sim.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,28 +16,33 @@
 from .supply import forecast_circulating_supply_df
 
 from .utils import validate_qap_method
 
 def setup_data_access(bearer_token_or_cfg: str):
     setup_spacescope(bearer_token_or_cfg)
 
+def validate_current_date(current_date: datetime.date):
+    if current_date > (datetime.date.today() - datetime.timedelta(days=2)):
+        raise ValueError("Current date must be at least 2 days in the past!")
+
 def run_simple_sim(
     start_date: datetime.date,
     current_date: datetime.date,
     forecast_length: int,
     renewal_rate: Union[np.array, float],
     rb_onboard_power: Union[np.array, float],
     fil_plus_rate: Union[np.array, float],
     duration: int,
     bearer_token_or_cfg: str,
     qap_method: str = 'basic' # can be set to tunable or basic
                               # see: https://hackmd.io/O6HmAb--SgmxkjLWSpbN_A?view
 ) -> pd.DataFrame:
     validate_qap_method(qap_method)
     setup_data_access(bearer_token_or_cfg)
+    validate_current_date(current_date)
 
     end_date = current_date + datetime.timedelta(days=forecast_length)
     # Get sector scheduled expirations
     res = get_sector_expiration_stats(start_date, current_date, end_date)
     rb_known_scheduled_expire_vec = res[0]
     qa_known_scheduled_expire_vec = res[1]
     known_scheduled_pledge_release_full_vec = res[2]
```

### Comparing `mechaFIL-1.7/mechafil/supply.py` & `mechaFIL-1.8/mechafil/supply.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     get_day_schedule_pledge_release,
     compute_day_reward_release,
     compute_day_delta_pledge,
     compute_day_locked_rewards,
     compute_day_locked_pledge,
 )
 from .power import scalar_or_vector_to_vector
+from .data import NETWORK_START
 
 """
 There is still a small discrepancy between the actual locked FIL and forecasted
 locked FIL. We believe that it could be due to the following reasons:
   a) Sector durations are not unlocked after exactly 1y. In general they're distributed and slightly longer. But in that case I’d expect the sign of the error to be the opposite to observed.
   b) The error between actual and forecasted locked FIL is 0 for day_idx=1. This might imply that a build up of errors due to an error in `day_locked_pledge` sounds more like it could be the issue.
   c) If we're sure the locking discrepancy is not a bug but rather a deficiency in the model popping up via the approximations used, we may way want to include a learnable factor to correct the difference
@@ -33,17 +34,17 @@
     burnt_fil_vec: np.array,
     vest_df: pd.DataFrame,
     mint_df: pd.DataFrame,
     known_scheduled_pledge_release_vec: np.array,
     lock_target: float = 0.3,
 ) -> pd.DataFrame:
     # we assume all stats started at main net launch, in 2020-10-15
-    start_day = (start_date - datetime.date(2020, 10, 15)).days
-    current_day = (current_date - datetime.date(2020, 10, 15)).days
-    end_day = (end_date - datetime.date(2020, 10, 15)).days
+    start_day = (start_date - NETWORK_START.date()).days
+    current_day = (current_date - NETWORK_START.date()).days
+    end_day = (end_date - NETWORK_START.date()).days
     # initialise dataframe and auxilialy variables
     df = initialise_circulating_supply_df(
         start_date,
         end_date,
         circ_supply_zero,
         locked_fil_zero,
         burnt_fil_vec,
```

### Comparing `mechaFIL-1.7/mechafil/vesting.py` & `mechaFIL-1.8/mechafil/vesting.py`

 * *Files identical despite different names*

### Comparing `mechaFIL-1.7/setup.py` & `mechaFIL-1.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mechaFIL",
-    version="1.7",
+    version="1.8",
     author="Maria Silva, Tom Mellan, Kiran Karra",
     author_email="misilva73@gmail.com, t.mellan@imperial.ac.uk, kiran.karra@gmail.com",
     description="Mechanistic model for the Filecoin Economy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         "Documentation": "https://github.com/protocol/filecoin-mecha-twin",
```

