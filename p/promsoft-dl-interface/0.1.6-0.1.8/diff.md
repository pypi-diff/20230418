# Comparing `tmp/promsoft_dl_interface-0.1.6.tar.gz` & `tmp/promsoft_dl_interface-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promsoft_dl_interface-0.1.6.tar", max compression
+gzip compressed data, was "promsoft_dl_interface-0.1.8.tar", max compression
```

## Comparing `promsoft_dl_interface-0.1.6.tar` & `promsoft_dl_interface-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      313 2023-04-14 08:20:00.624386 promsoft_dl_interface-0.1.6/README.md
--rw-r--r--   0        0        0      407 2023-04-06 14:33:31.145236 promsoft_dl_interface-0.1.6/dl_interface/__init__.py
--rw-r--r--   0        0        0     2592 2023-04-06 14:33:31.145236 promsoft_dl_interface-0.1.6/dl_interface/models.py
--rw-r--r--   0        0        0     3630 2023-04-06 14:33:31.145236 promsoft_dl_interface-0.1.6/dl_interface/request.py
--rw-r--r--   0        0        0      526 2023-04-14 08:20:00.624386 promsoft_dl_interface-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 promsoft_dl_interface-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      313 2023-04-14 07:44:38.776194 promsoft_dl_interface-0.1.8/README.md
+-rw-r--r--   0        0        0      407 2023-04-06 14:10:59.360316 promsoft_dl_interface-0.1.8/dl_interface/__init__.py
+-rw-r--r--   0        0        0     2592 2023-04-06 14:10:59.360316 promsoft_dl_interface-0.1.8/dl_interface/models.py
+-rw-r--r--   0        0        0     3630 2023-04-06 14:10:59.364316 promsoft_dl_interface-0.1.8/dl_interface/request.py
+-rw-r--r--   0        0        0      504 2023-04-18 05:45:05.722780 promsoft_dl_interface-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 promsoft_dl_interface-0.1.8/PKG-INFO
```

### Comparing `promsoft_dl_interface-0.1.6/dl_interface/models.py` & `promsoft_dl_interface-0.1.8/dl_interface/models.py`

 * *Files identical despite different names*

### Comparing `promsoft_dl_interface-0.1.6/dl_interface/request.py` & `promsoft_dl_interface-0.1.8/dl_interface/request.py`

 * *Files identical despite different names*

### Comparing `promsoft_dl_interface-0.1.6/PKG-INFO` & `promsoft_dl_interface-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: promsoft-dl-interface
-Version: 0.1.6
+Version: 0.1.8
 Summary: Интерфейс HTTP API транспортной компании Деловые линии.
-Author: Oleg
-Author-email: olegspk@promsosft.ru
+Author: Promsoft
+Author-email: info@promsoft.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: promsoft-dl-interface Version: 0.1.6 Summary:
+Metadata-Version: 2.1 Name: promsoft-dl-interface Version: 0.1.8 Summary:
 ÐÐ½ÑÐµÑÑÐµÐ¹Ñ HTTP API ÑÑÐ°Ð½ÑÐ¿Ð¾ÑÑÐ½Ð¾Ð¹ ÐºÐ¾Ð¼Ð¿Ð°Ð½Ð¸Ð¸
-ÐÐµÐ»Ð¾Ð²ÑÐµ Ð»Ð¸Ð½Ð¸Ð¸. Author: Oleg Author-email: olegspk@promsosft.ru
+ÐÐµÐ»Ð¾Ð²ÑÐµ Ð»Ð¸Ð½Ð¸Ð¸. Author: Promsoft Author-email: info@promsoft.ru
 Requires-Python: >=3.10,<4.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Description-Content-Type: text/markdown Interfaces for API Delovie_linii
 transport company. Usage: ``` from dl_interface import Counteragent ca =
 Counteragent(form="0xb9090c56d0e15e524e2035fcea921d4d", name="ÐÐ²Ð°Ð½Ð¾Ð²
 ÐÐ²Ð°Ð½ ÐÐ²Ð°Ð½Ð¾Ð²Ð¸Ñ") print(f"As dict: {ca.dict()}") ```
```

