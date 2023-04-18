# Comparing `tmp/iamai_adapter_apscheduler-0.6.0.tar.gz` & `tmp/iamai_adapter_apscheduler-0.6.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamai_adapter_apscheduler-0.6.0.tar", max compression
+gzip compressed data, was "iamai_adapter_apscheduler-0.6.0.post1.tar", max compression
```

## Comparing `iamai_adapter_apscheduler-0.6.0.tar` & `iamai_adapter_apscheduler-0.6.0.post1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-04-05 06:03:03.805478 iamai_adapter_apscheduler-0.6.0/README.md
--rw-r--r--   0        0        0     4674 2023-04-05 06:03:03.805478 iamai_adapter_apscheduler-0.6.0/iamai/adapter/apscheduler/__init__.py
--rw-r--r--   0        0        0      377 2023-04-05 06:03:03.805478 iamai_adapter_apscheduler-0.6.0/iamai/adapter/apscheduler/config.py
--rw-r--r--   0        0        0      932 2023-04-05 06:03:03.805478 iamai_adapter_apscheduler-0.6.0/iamai/adapter/apscheduler/event.py
--rw-r--r--   0        0        0     1331 2023-04-05 06:03:03.805478 iamai_adapter_apscheduler-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1122 1970-01-01 00:00:00.000000 iamai_adapter_apscheduler-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-18 16:36:06.706341 iamai_adapter_apscheduler-0.6.0.post1/README.md
+-rw-r--r--   0        0        0     4675 2023-04-18 16:36:06.706341 iamai_adapter_apscheduler-0.6.0.post1/iamai/adapter/apscheduler/__init__.py
+-rw-r--r--   0        0        0      377 2023-04-18 16:36:06.706341 iamai_adapter_apscheduler-0.6.0.post1/iamai/adapter/apscheduler/config.py
+-rw-r--r--   0        0        0      932 2023-04-18 16:36:06.706341 iamai_adapter_apscheduler-0.6.0.post1/iamai/adapter/apscheduler/event.py
+-rw-r--r--   0        0        0     1337 2023-04-18 16:36:06.706341 iamai_adapter_apscheduler-0.6.0.post1/pyproject.toml
+-rw-r--r--   0        0        0     1128 1970-01-01 00:00:00.000000 iamai_adapter_apscheduler-0.6.0.post1/PKG-INFO
```

### Comparing `iamai_adapter_apscheduler-0.6.0/iamai/adapter/apscheduler/__init__.py` & `iamai_adapter_apscheduler-0.6.0.post1/iamai/adapter/apscheduler/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 """
 import asyncio
 import inspect
 from functools import wraps
 from typing import Any, Dict, Type
 
 from apscheduler.job import Job
+from apscheduler.schedulers.asyncio import AsyncIOScheduler
+
 from iamai.plugin import Plugin
 from iamai.adapter import Adapter
 from iamai.log import logger, error_or_exception
-from apscheduler.schedulers.asyncio import AsyncIOScheduler
 
 from .config import Config
 from .event import APSchedulerEvent
 
 __all__ = ["APSchedulerAdapter", "scheduler_decorator"]
```

### Comparing `iamai_adapter_apscheduler-0.6.0/iamai/adapter/apscheduler/event.py` & `iamai_adapter_apscheduler-0.6.0.post1/iamai/adapter/apscheduler/event.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_apscheduler-0.6.0/pyproject.toml` & `iamai_adapter_apscheduler-0.6.0.post1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iamai-adapter-apscheduler"
-version = "0.6.0"
+version = "0.6.0.post1"
 description = "APScheduler adapter for iamai."
 authors = ["简律纯 <admin@jyunko.cn>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://retrofor.space/"
 repository = "https://github.com/retrofor/iamai"
 documentation = "https://iamai.retrofor.space/"
```

### Comparing `iamai_adapter_apscheduler-0.6.0/PKG-INFO` & `iamai_adapter_apscheduler-0.6.0.post1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamai-adapter-apscheduler
-Version: 0.6.0
+Version: 0.6.0.post1
 Summary: APScheduler adapter for iamai.
 Home-page: https://retrofor.space/
 License: MIT
 Keywords: bot,chatbot,scheduling,apscheduler
 Author: 简律纯
 Author-email: admin@jyunko.cn
 Requires-Python: >=3.8,<4.0
```

