# Comparing `tmp/iamai_adapter_dingtalk-0.6.0.tar.gz` & `tmp/iamai_adapter_dingtalk-0.6.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamai_adapter_dingtalk-0.6.0.tar", max compression
+gzip compressed data, was "iamai_adapter_dingtalk-0.6.0.post1.tar", max compression
```

## Comparing `iamai_adapter_dingtalk-0.6.0.tar` & `iamai_adapter_dingtalk-0.6.0.post1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-04-05 06:03:03.805478 iamai_adapter_dingtalk-0.6.0/README.md
--rw-r--r--   0        0        0     5439 2023-04-05 06:03:03.805478 iamai_adapter_dingtalk-0.6.0/iamai/adapter/dingtalk/__init__.py
--rw-r--r--   0        0        0      590 2023-04-05 06:03:03.805478 iamai_adapter_dingtalk-0.6.0/iamai/adapter/dingtalk/config.py
--rw-r--r--   0        0        0     2362 2023-04-05 06:03:03.805478 iamai_adapter_dingtalk-0.6.0/iamai/adapter/dingtalk/event.py
--rw-r--r--   0        0        0      387 2023-04-05 06:03:03.805478 iamai_adapter_dingtalk-0.6.0/iamai/adapter/dingtalk/exceptions.py
--rw-r--r--   0        0        0     3200 2023-04-05 06:03:03.805478 iamai_adapter_dingtalk-0.6.0/iamai/adapter/dingtalk/message.py
--rw-r--r--   0        0        0     1287 2023-04-05 06:03:03.805478 iamai_adapter_dingtalk-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1062 1970-01-01 00:00:00.000000 iamai_adapter_dingtalk-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-18 16:36:06.706341 iamai_adapter_dingtalk-0.6.0.post1/README.md
+-rw-r--r--   0        0        0     5440 2023-04-18 16:36:06.706341 iamai_adapter_dingtalk-0.6.0.post1/iamai/adapter/dingtalk/__init__.py
+-rw-r--r--   0        0        0      590 2023-04-18 16:36:06.706341 iamai_adapter_dingtalk-0.6.0.post1/iamai/adapter/dingtalk/config.py
+-rw-r--r--   0        0        0     2363 2023-04-18 16:36:06.706341 iamai_adapter_dingtalk-0.6.0.post1/iamai/adapter/dingtalk/event.py
+-rw-r--r--   0        0        0      387 2023-04-18 16:36:06.706341 iamai_adapter_dingtalk-0.6.0.post1/iamai/adapter/dingtalk/exceptions.py
+-rw-r--r--   0        0        0     3200 2023-04-18 16:36:06.706341 iamai_adapter_dingtalk-0.6.0.post1/iamai/adapter/dingtalk/message.py
+-rw-r--r--   0        0        0     1293 2023-04-18 16:36:06.706341 iamai_adapter_dingtalk-0.6.0.post1/pyproject.toml
+-rw-r--r--   0        0        0     1068 1970-01-01 00:00:00.000000 iamai_adapter_dingtalk-0.6.0.post1/PKG-INFO
```

### Comparing `iamai_adapter_dingtalk-0.6.0/iamai/adapter/dingtalk/__init__.py` & `iamai_adapter_dingtalk-0.6.0.post1/iamai/adapter/dingtalk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import time
 import base64
 import hashlib
 from typing import Any, Dict, Union, Literal
 
 import aiohttp
 from aiohttp import web
+
 from iamai.adapter import Adapter
 from iamai.log import logger, error_or_exception
 
 from .config import Config
 from .event import DingTalkEvent
 from .message import DingTalkMessage
 from .exceptions import ApiTimeout, NetworkError
```

### Comparing `iamai_adapter_dingtalk-0.6.0/iamai/adapter/dingtalk/config.py` & `iamai_adapter_dingtalk-0.6.0.post1/iamai/adapter/dingtalk/config.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_dingtalk-0.6.0/iamai/adapter/dingtalk/event.py` & `iamai_adapter_dingtalk-0.6.0.post1/iamai/adapter/dingtalk/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """DingTalk 适配器事件。"""
 import time
 from typing import TYPE_CHECKING, Any, Dict, List, Union, Literal, Optional
 
-from iamai.event import Event
 from pydantic import Field, BaseModel, validator
 
+from iamai.event import Event
+
 from .message import DingTalkMessage
 from .exceptions import WebhookExpiredError
 
 if TYPE_CHECKING:
     from . import DingTalkAdapter  # noqa
```

### Comparing `iamai_adapter_dingtalk-0.6.0/iamai/adapter/dingtalk/message.py` & `iamai_adapter_dingtalk-0.6.0.post1/iamai/adapter/dingtalk/message.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_dingtalk-0.6.0/pyproject.toml` & `iamai_adapter_dingtalk-0.6.0.post1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iamai-adapter-dingtalk"
-version = "0.6.0"
+version = "0.6.0.post1"
 description = "DingTalk adapter for iamai."
 authors = ["简律纯 <admin@jyunko.cn>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://retrofor.space/"
 repository = "https://github.com/retrofor/iamai"
 documentation = "https://iamai.retrofor.space/"
```

### Comparing `iamai_adapter_dingtalk-0.6.0/PKG-INFO` & `iamai_adapter_dingtalk-0.6.0.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamai-adapter-dingtalk
-Version: 0.6.0
+Version: 0.6.0.post1
 Summary: DingTalk adapter for iamai.
 Home-page: https://retrofor.space/
 License: MIT
 Keywords: bot,chatbot,dingtalk
 Author: 简律纯
 Author-email: admin@jyunko.cn
 Requires-Python: >=3.8,<4.0
```

