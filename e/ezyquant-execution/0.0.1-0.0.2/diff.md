# Comparing `tmp/ezyquant-execution-0.0.1.tar.gz` & `tmp/ezyquant-execution-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezyquant-execution-0.0.1.tar", last modified: Thu Mar  2 10:26:37 2023, max compression
+gzip compressed data, was "ezyquant-execution-0.0.2.tar", last modified: Tue Apr 18 07:50:37 2023, max compression
```

## Comparing `ezyquant-execution-0.0.1.tar` & `ezyquant-execution-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:26:37.646374 ezyquant-execution-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-03-02 10:26:22.000000 ezyquant-execution-0.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-03-02 10:26:37.646374 ezyquant-execution-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-02 10:26:22.000000 ezyquant-execution-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:26:37.646374 ezyquant-execution-0.0.1/ezyquant_execution/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-02 10:26:22.000000 ezyquant-execution-0.0.1/ezyquant_execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-02 10:26:22.000000 ezyquant-execution-0.0.1/ezyquant_execution/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-03-02 10:26:22.000000 ezyquant-execution-0.0.1/ezyquant_execution/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)    14078 2023-03-02 10:26:22.000000 ezyquant-execution-0.0.1/ezyquant_execution/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-03-02 10:26:22.000000 ezyquant-execution-0.0.1/ezyquant_execution/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-03-02 10:26:22.000000 ezyquant-execution-0.0.1/ezyquant_execution/executing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-03-02 10:26:22.000000 ezyquant-execution-0.0.1/ezyquant_execution/realtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-03-02 10:26:22.000000 ezyquant-execution-0.0.1/ezyquant_execution/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 10:26:37.646374 ezyquant-execution-0.0.1/ezyquant_execution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-03-02 10:26:37.000000 ezyquant-execution-0.0.1/ezyquant_execution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-03-02 10:26:37.000000 ezyquant-execution-0.0.1/ezyquant_execution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 10:26:37.000000 ezyquant-execution-0.0.1/ezyquant_execution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-02 10:26:37.000000 ezyquant-execution-0.0.1/ezyquant_execution.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-02 10:26:37.000000 ezyquant-execution-0.0.1/ezyquant_execution.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-02 10:26:37.646374 ezyquant-execution-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-03-02 10:26:22.000000 ezyquant-execution-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:50:37.427486 ezyquant-execution-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-18 07:50:20.000000 ezyquant-execution-0.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-18 07:50:37.427486 ezyquant-execution-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-18 07:50:20.000000 ezyquant-execution-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:50:37.427486 ezyquant-execution-0.0.2/ezyquant_execution/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-18 07:50:20.000000 ezyquant-execution-0.0.2/ezyquant_execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 07:50:20.000000 ezyquant-execution-0.0.2/ezyquant_execution/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-18 07:50:20.000000 ezyquant-execution-0.0.2/ezyquant_execution/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14364 2023-04-18 07:50:20.000000 ezyquant-execution-0.0.2/ezyquant_execution/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-04-18 07:50:20.000000 ezyquant-execution-0.0.2/ezyquant_execution/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-04-18 07:50:20.000000 ezyquant-execution-0.0.2/ezyquant_execution/executing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-18 07:50:20.000000 ezyquant-execution-0.0.2/ezyquant_execution/realtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-18 07:50:20.000000 ezyquant-execution-0.0.2/ezyquant_execution/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:50:37.427486 ezyquant-execution-0.0.2/ezyquant_execution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-18 07:50:37.000000 ezyquant-execution-0.0.2/ezyquant_execution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-18 07:50:37.000000 ezyquant-execution-0.0.2/ezyquant_execution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:50:37.000000 ezyquant-execution-0.0.2/ezyquant_execution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-18 07:50:37.000000 ezyquant-execution-0.0.2/ezyquant_execution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-18 07:50:37.000000 ezyquant-execution-0.0.2/ezyquant_execution.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-18 07:50:37.427486 ezyquant-execution-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-18 07:50:20.000000 ezyquant-execution-0.0.2/setup.py
```

### Comparing `ezyquant-execution-0.0.1/LICENSE.txt` & `ezyquant-execution-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.0.1/PKG-INFO` & `ezyquant-execution-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezyquant-execution
-Version: 0.0.1
+Version: 0.0.2
 Summary: Ezyquant execution
 Home-page: https://pydoc.ezyquant.com/
 Author: Fintech (Thailand) Company Limited
 Author-email: admin@fintech.co.th
 Maintainer: Fintech (Thailand) Company Limited
 Maintainer-email: admin@fintech.co.th
 License: The MIT License (MIT)
```

### Comparing `ezyquant-execution-0.0.1/ezyquant_execution/constant.py` & `ezyquant-execution-0.0.2/ezyquant_execution/constant.py`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.0.1/ezyquant_execution/context.py` & `ezyquant-execution-0.0.2/ezyquant_execution/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import time as t
 import warnings
 from dataclasses import dataclass
 from datetime import datetime
-from functools import cached_property
+from functools import cached_property, lru_cache
 from typing import Any, Callable, Dict, List, Optional, TypeVar, Union
 
 import pandas as pd
 from settrade_v2.context import Context
 from settrade_v2.equity import InvestorEquity, MarketRepEquity
 from settrade_v2.market import MarketData
 from settrade_v2.realtime import RealtimeDataConnection
-from settrade_v2.user import Investor, MarketRep
+from settrade_v2.user import Investor, MarketRep, _BaseUser
 
 from . import utils
 from .entity import (
     PRICE_TYPE,
     SIDE_BUY,
     SIDE_SELL,
     SIDE_TYPE,
@@ -25,14 +25,21 @@
     EquityPortfolio,
     EquityTrade,
     PortfolioResponse,
     StockQuoteResponse,
 )
 from .realtime import BidOfferSubscriber, PriceInfoSubscriber
 
+# Override _BaseUser.RealtimeDataConnection
+# because subscribe will error if init RealtimeDataConnection more than once
+# Can remove this line if this issue is fixed
+_BaseUser.RealtimeDataConnection = lru_cache(maxsize=1)(
+    _BaseUser.RealtimeDataConnection
+)
+
 T = TypeVar("T")
 
 
 def new_refresh(self):
     res = self.request(
         "POST",
         self.refresh_token_path,
```

### Comparing `ezyquant-execution-0.0.1/ezyquant_execution/entity.py` & `ezyquant-execution-0.0.2/ezyquant_execution/entity.py`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.0.1/ezyquant_execution/executing.py` & `ezyquant-execution-0.0.2/ezyquant_execution/executing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import asyncio
 from datetime import time
 from threading import Event, Timer
-from typing import Any, Callable, Dict, Optional, Union
+from typing import Any, Awaitable, Callable, Dict, Optional, Union
 
 from settrade_v2.user import Investor, MarketRep
 
 from . import utils
 from .context import ExecuteContext
 
 
@@ -72,7 +73,50 @@
         while not event.wait(interval):
             [on_timer(i) for i in ctx_list]
 
     finally:
         # note that event.set() and timer.cancel() can be called multiple times
         event.set()
         timer.cancel()
+
+
+async def async_execute_on_timer(
+    settrade_user: Union[Investor, MarketRep],
+    account_no: str,
+    signal_dict: Dict[str, Any],
+    on_timer: Callable[[ExecuteContext], Awaitable[None]],
+    interval: float,
+    start_time: time,
+    end_time: time,
+    pin: Optional[str] = None,
+    event: Optional[asyncio.Event] = None,
+):
+    """Same as execute_on_timer but on_timer is async function."""
+    if event is None:
+        event = asyncio.Event()
+
+    # sleep until start time
+    await utils.async_sleep_until(start_time, event=event)
+
+    timer = Timer(utils.seconds_until(end_time), event.set)
+    timer.start()
+
+    try:
+        ctx_list = [
+            ExecuteContext(
+                symbol=k,
+                signal=v,
+                settrade_user=settrade_user,
+                account_no=account_no,
+                pin=pin,
+            )
+            for k, v in signal_dict.items()
+        ]
+
+        # execute on_timer
+        while not await utils.async_event_wait(event, interval):
+            [await on_timer(i) for i in ctx_list]
+
+    finally:
+        # note that event.set() and timer.cancel() can be called multiple times
+        event.set()
+        timer.cancel()
```

### Comparing `ezyquant-execution-0.0.1/ezyquant_execution/realtime.py` & `ezyquant-execution-0.0.2/ezyquant_execution/realtime.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 from threading import Event
-from typing import Callable
+from typing import Callable, Optional
 
-from settrade_v2.realtime import RealtimeDataConnection
+from settrade_v2.realtime import RealtimeDataConnection, Subscriber
 
 from .entity import BidOffer, PriceInfo
 
 
 class SettradeSubscriber:
-    def __init__(self, function: Callable, *args, **kwargs):
+    def __init__(self, function: Callable[..., Subscriber], *args, **kwargs):
         self.function = function
         self.args = args
         self.kwargs = kwargs
 
-        self._data: dict = {}
+        self._data: Optional[dict] = {}
+        self._error: Optional[Exception] = None
 
         self._event: Event = Event()
         self.function(on_message=self._on_message, *self.args, **self.kwargs).start()
-        self._event.wait()  # wait for first update
+        self._event.wait(timeout=30)  # wait for first update
 
     @property
     def data(self) -> dict:
+        if self._error:
+            raise self._error
+        if self._data is None:
+            raise ConnectionError("No data received yet")
         return self._data
 
     def _on_message(self, message):
+        self._event.set()
         if message["is_success"]:
             self._data = message["data"]
-            self._event.set()
+            self._error = None
         else:
-            raise ConnectionError(message["message"])
+            self._error = ConnectionError(message["message"])
+            raise self._error
 
 
 class BidOfferSubscriber(SettradeSubscriber):
     def __init__(self, symbol: str, rt_conn: RealtimeDataConnection):
         super().__init__(rt_conn.subscribe_bid_offer, symbol=symbol)
 
     @property
```

### Comparing `ezyquant-execution-0.0.1/ezyquant_execution.egg-info/PKG-INFO` & `ezyquant-execution-0.0.2/ezyquant_execution.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezyquant-execution
-Version: 0.0.1
+Version: 0.0.2
 Summary: Ezyquant execution
 Home-page: https://pydoc.ezyquant.com/
 Author: Fintech (Thailand) Company Limited
 Author-email: admin@fintech.co.th
 Maintainer: Fintech (Thailand) Company Limited
 Maintainer-email: admin@fintech.co.th
 License: The MIT License (MIT)
```

### Comparing `ezyquant-execution-0.0.1/setup.py` & `ezyquant-execution-0.0.2/setup.py`

 * *Files identical despite different names*

