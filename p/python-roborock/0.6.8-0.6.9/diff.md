# Comparing `tmp/python_roborock-0.6.8.tar.gz` & `tmp/python_roborock-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_roborock-0.6.8.tar", max compression
+gzip compressed data, was "python_roborock-0.6.9.tar", max compression
```

## Comparing `python_roborock-0.6.8.tar` & `python_roborock-0.6.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2023-04-18 01:25:32.510693 python_roborock-0.6.8/LICENSE
--rw-r--r--   0        0        0     2122 2023-04-18 01:25:32.510693 python_roborock-0.6.8/README.md
--rw-r--r--   0        0        0     1370 2023-04-18 01:25:33.214690 python_roborock-0.6.8/pyproject.toml
--rw-r--r--   0        0        0      156 2023-04-18 01:25:32.510693 python_roborock-0.6.8/roborock/__init__.py
--rw-r--r--   0        0        0    18701 2023-04-18 01:25:32.510693 python_roborock-0.6.8/roborock/api.py
--rw-r--r--   0        0        0     3991 2023-04-18 01:25:32.514693 python_roborock-0.6.8/roborock/cli.py
--rw-r--r--   0        0        0     8380 2023-04-18 01:25:32.514693 python_roborock-0.6.8/roborock/cloud_api.py
--rw-r--r--   0        0        0     4283 2023-04-18 01:25:32.514693 python_roborock-0.6.8/roborock/code_mappings.py
--rw-r--r--   0        0        0     9404 2023-04-18 01:25:32.514693 python_roborock-0.6.8/roborock/containers.py
--rw-r--r--   0        0        0     1028 2023-04-18 01:25:32.514693 python_roborock-0.6.8/roborock/exceptions.py
--rw-r--r--   0        0        0     7214 2023-04-18 01:25:32.514693 python_roborock-0.6.8/roborock/local_api.py
--rw-r--r--   0        0        0      618 2023-04-18 01:25:32.514693 python_roborock-0.6.8/roborock/roborock_future.py
--rw-r--r--   0        0        0     6108 2023-04-18 01:25:32.514693 python_roborock-0.6.8/roborock/roborock_message.py
--rw-r--r--   0        0        0    12762 2023-04-18 01:25:32.514693 python_roborock-0.6.8/roborock/typing.py
--rw-r--r--   0        0        0      567 2023-04-18 01:25:32.514693 python_roborock-0.6.8/roborock/util.py
--rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 python_roborock-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-18 01:34:40.571646 python_roborock-0.6.9/LICENSE
+-rw-r--r--   0        0        0     2122 2023-04-18 01:34:40.571646 python_roborock-0.6.9/README.md
+-rw-r--r--   0        0        0     1370 2023-04-18 01:34:41.475658 python_roborock-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-04-18 01:34:40.571646 python_roborock-0.6.9/roborock/__init__.py
+-rw-r--r--   0        0        0    18700 2023-04-18 01:34:40.571646 python_roborock-0.6.9/roborock/api.py
+-rw-r--r--   0        0        0     3991 2023-04-18 01:34:40.571646 python_roborock-0.6.9/roborock/cli.py
+-rw-r--r--   0        0        0     8380 2023-04-18 01:34:40.571646 python_roborock-0.6.9/roborock/cloud_api.py
+-rw-r--r--   0        0        0     4283 2023-04-18 01:34:40.571646 python_roborock-0.6.9/roborock/code_mappings.py
+-rw-r--r--   0        0        0     9404 2023-04-18 01:34:40.571646 python_roborock-0.6.9/roborock/containers.py
+-rw-r--r--   0        0        0     1028 2023-04-18 01:34:40.571646 python_roborock-0.6.9/roborock/exceptions.py
+-rw-r--r--   0        0        0     7198 2023-04-18 01:34:40.571646 python_roborock-0.6.9/roborock/local_api.py
+-rw-r--r--   0        0        0      618 2023-04-18 01:34:40.571646 python_roborock-0.6.9/roborock/roborock_future.py
+-rw-r--r--   0        0        0     6108 2023-04-18 01:34:40.571646 python_roborock-0.6.9/roborock/roborock_message.py
+-rw-r--r--   0        0        0    12762 2023-04-18 01:34:40.571646 python_roborock-0.6.9/roborock/typing.py
+-rw-r--r--   0        0        0      567 2023-04-18 01:34:40.571646 python_roborock-0.6.9/roborock/util.py
+-rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 python_roborock-0.6.9/PKG-INFO
```

### Comparing `python_roborock-0.6.8/LICENSE` & `python_roborock-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.8/README.md` & `python_roborock-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.8/pyproject.toml` & `python_roborock-0.6.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-roborock"
-version = "0.6.8"
+version = "0.6.9"
 description = "A package to control Roborock vacuums."
 authors = ["humbertogontijo <humbertogontijo@users.noreply.github.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/humbertogontijo/python-roborock"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `python_roborock-0.6.8/roborock/api.py` & `python_roborock-0.6.9/roborock/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from typing import Any, Callable, Coroutine, Mapping, Optional
 
 import aiohttp
 from Crypto.Cipher import AES
 from Crypto.Util.Padding import unpad
 
 from roborock.exceptions import RoborockException, RoborockTimeout, VacuumError
-
 from .code_mappings import RoborockDockTypeCode, RoborockEnum
 from .containers import (
     CleanRecord,
     CleanSummary,
     Consumable,
     DNDTimer,
     DustCollectionMode,
@@ -34,16 +33,16 @@
     NetworkInfo,
     RoborockDeviceInfo,
     SmartWashParams,
     Status,
     UserData,
     WashTowelMode,
 )
-from .roborock_message import RoborockMessage
 from .roborock_future import RoborockFuture
+from .roborock_message import RoborockMessage
 from .typing import RoborockCommand, RoborockDeviceProp, RoborockDockSummary
 
 _LOGGER = logging.getLogger(__name__)
 QUEUE_TIMEOUT = 4
 SPECIAL_COMMANDS = [
     RoborockCommand.GET_MAP_V1,
 ]
```

### Comparing `python_roborock-0.6.8/roborock/cli.py` & `python_roborock-0.6.9/roborock/cli.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.8/roborock/cloud_api.py` & `python_roborock-0.6.9/roborock/cloud_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.8/roborock/code_mappings.py` & `python_roborock-0.6.9/roborock/code_mappings.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.8/roborock/containers.py` & `python_roborock-0.6.9/roborock/containers.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.8/roborock/exceptions.py` & `python_roborock-0.6.9/roborock/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.8/roborock/local_api.py` & `python_roborock-0.6.9/roborock/local_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 import socket
 from asyncio import Lock
-from typing import Any, Awaitable, Callable, Mapping, Optional
+from typing import Callable, Mapping, Optional
 
 import async_timeout
 
 from roborock.api import SPECIAL_COMMANDS, RoborockClient
 from roborock.containers import RoborockLocalDeviceInfo
 from roborock.exceptions import CommandVacuumError, RoborockConnectionException, RoborockException, RoborockTimeout
 from roborock.roborock_message import RoborockMessage, RoborockParser
```

### Comparing `python_roborock-0.6.8/roborock/roborock_future.py` & `python_roborock-0.6.9/roborock/roborock_future.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.8/roborock/roborock_message.py` & `python_roborock-0.6.9/roborock/roborock_message.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.8/roborock/typing.py` & `python_roborock-0.6.9/roborock/typing.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.8/roborock/util.py` & `python_roborock-0.6.9/roborock/util.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.8/PKG-INFO` & `python_roborock-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-roborock
-Version: 0.6.8
+Version: 0.6.9
 Summary: A package to control Roborock vacuums.
 Home-page: https://github.com/humbertogontijo/python-roborock
 License: GPL-3.0-only
 Author: humbertogontijo
 Author-email: humbertogontijo@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-roborock Version: 0.6.8 Summary: A package
+Metadata-Version: 2.1 Name: python-roborock Version: 0.6.9 Summary: A package
 to control Roborock vacuums. Home-page: https://github.com/humbertogontijo/
 python-roborock License: GPL-3.0-only Author: humbertogontijo Author-email:
 humbertogontijo@users.noreply.github.com Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

