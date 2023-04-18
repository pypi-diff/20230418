# Comparing `tmp/iamai_adapter_mirai-0.6.0.post2.tar.gz` & `tmp/iamai_adapter_mirai-0.6.0.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamai_adapter_mirai-0.6.0.post2.tar", max compression
+gzip compressed data, was "iamai_adapter_mirai-0.6.0.post3.tar", max compression
```

## Comparing `iamai_adapter_mirai-0.6.0.post2.tar` & `iamai_adapter_mirai-0.6.0.post3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34522 2023-04-05 06:03:03.805478 iamai_adapter_mirai-0.6.0.post2/LICENSE
--rw-r--r--   0        0        0      242 2023-04-05 06:03:03.805478 iamai_adapter_mirai-0.6.0.post2/README.md
--rw-r--r--   0        0        0     9055 2023-04-05 06:03:03.805478 iamai_adapter_mirai-0.6.0.post2/iamai/adapter/mirai/__init__.py
--rw-r--r--   0        0        0     1029 2023-04-05 06:03:03.805478 iamai_adapter_mirai-0.6.0.post2/iamai/adapter/mirai/config.py
--rw-r--r--   0        0        0      562 2023-04-05 06:03:03.805478 iamai_adapter_mirai-0.6.0.post2/iamai/adapter/mirai/event/__init__.py
--rw-r--r--   0        0        0      822 2023-04-05 06:03:03.805478 iamai_adapter_mirai-0.6.0.post2/iamai/adapter/mirai/event/base.py
--rw-r--r--   0        0        0     1042 2023-04-05 06:03:03.805478 iamai_adapter_mirai-0.6.0.post2/iamai/adapter/mirai/event/mate.py
--rw-r--r--   0        0        0     3650 2023-04-05 06:03:03.805478 iamai_adapter_mirai-0.6.0.post2/iamai/adapter/mirai/event/message.py
--rw-r--r--   0        0        0     5492 2023-04-05 06:03:03.805478 iamai_adapter_mirai-0.6.0.post2/iamai/adapter/mirai/event/notice.py
--rw-r--r--   0        0        0     4264 2023-04-05 06:03:03.805478 iamai_adapter_mirai-0.6.0.post2/iamai/adapter/mirai/event/request.py
--rw-r--r--   0        0        0      644 2023-04-05 06:03:03.805478 iamai_adapter_mirai-0.6.0.post2/iamai/adapter/mirai/exceptions.py
--rw-r--r--   0        0        0     4419 2023-04-05 06:03:03.805478 iamai_adapter_mirai-0.6.0.post2/iamai/adapter/mirai/message.py
--rw-r--r--   0        0        0     1300 2023-04-05 06:03:03.805478 iamai_adapter_mirai-0.6.0.post2/pyproject.toml
--rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 iamai_adapter_mirai-0.6.0.post2/PKG-INFO
+-rw-r--r--   0        0        0    34522 2023-04-18 16:36:06.706341 iamai_adapter_mirai-0.6.0.post3/LICENSE
+-rw-r--r--   0        0        0      242 2023-04-18 16:36:06.706341 iamai_adapter_mirai-0.6.0.post3/README.md
+-rw-r--r--   0        0        0     9055 2023-04-18 16:36:06.706341 iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/__init__.py
+-rw-r--r--   0        0        0     1029 2023-04-18 16:36:06.706341 iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/config.py
+-rw-r--r--   0        0        0      562 2023-04-18 16:36:06.706341 iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/event/__init__.py
+-rw-r--r--   0        0        0      822 2023-04-18 16:36:06.706341 iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/event/base.py
+-rw-r--r--   0        0        0     1042 2023-04-18 16:36:06.706341 iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/event/mate.py
+-rw-r--r--   0        0        0     3650 2023-04-18 16:36:06.706341 iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/event/message.py
+-rw-r--r--   0        0        0     5492 2023-04-18 16:36:06.706341 iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/event/notice.py
+-rw-r--r--   0        0        0     4264 2023-04-18 16:36:06.706341 iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/event/request.py
+-rw-r--r--   0        0        0      644 2023-04-18 16:36:06.706341 iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/exceptions.py
+-rw-r--r--   0        0        0     4419 2023-04-18 16:36:06.706341 iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/message.py
+-rw-r--r--   0        0        0     1300 2023-04-18 16:36:06.706341 iamai_adapter_mirai-0.6.0.post3/pyproject.toml
+-rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 iamai_adapter_mirai-0.6.0.post3/PKG-INFO
```

### Comparing `iamai_adapter_mirai-0.6.0.post2/LICENSE` & `iamai_adapter_mirai-0.6.0.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-0.6.0.post2/iamai/adapter/mirai/__init__.py` & `iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/__init__.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-0.6.0.post2/iamai/adapter/mirai/config.py` & `iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/config.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-0.6.0.post2/iamai/adapter/mirai/event/__init__.py` & `iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/event/__init__.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-0.6.0.post2/iamai/adapter/mirai/event/base.py` & `iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/event/base.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-0.6.0.post2/iamai/adapter/mirai/event/mate.py` & `iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/event/mate.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-0.6.0.post2/iamai/adapter/mirai/event/message.py` & `iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/event/message.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-0.6.0.post2/iamai/adapter/mirai/event/notice.py` & `iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/event/notice.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-0.6.0.post2/iamai/adapter/mirai/event/request.py` & `iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/event/request.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-0.6.0.post2/iamai/adapter/mirai/exceptions.py` & `iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/exceptions.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-0.6.0.post2/iamai/adapter/mirai/message.py` & `iamai_adapter_mirai-0.6.0.post3/iamai/adapter/mirai/message.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_mirai-0.6.0.post2/pyproject.toml` & `iamai_adapter_mirai-0.6.0.post3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iamai-adapter-mirai"
-version = "0.6.0.post2"
+version = "0.6.0.post3"
 description = "Mirai adapter for iamai."
 authors = ["简律纯 <admin@jyunko.cn>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://retrofor.space/"
 repository = "https://github.com/retrofor/iamai"
 documentation = "https://iamai.retrofor.space/"
```

### Comparing `iamai_adapter_mirai-0.6.0.post2/PKG-INFO` & `iamai_adapter_mirai-0.6.0.post3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamai-adapter-mirai
-Version: 0.6.0.post2
+Version: 0.6.0.post3
 Summary: Mirai adapter for iamai.
 Home-page: https://retrofor.space/
 License: MIT
 Keywords: bot,chatbot,qq,qqbot,mirai
 Author: 简律纯
 Author-email: admin@jyunko.cn
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iamai-adapter-mirai Version: 0.6.0.post2 Summary:
+Metadata-Version: 2.1 Name: iamai-adapter-mirai Version: 0.6.0.post3 Summary:
 Mirai adapter for iamai. Home-page: https://retrofor.space/ License: MIT
 Keywords: bot,chatbot,qq,qqbot,mirai Author: ç®å¾çº¯ Author-email:
 admin@jyunko.cn Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 3
 - Alpha Classifier: Framework :: AsyncIO Classifier: Framework :: Robot
 Framework Classifier: Framework :: Robot Framework :: Library Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
```

