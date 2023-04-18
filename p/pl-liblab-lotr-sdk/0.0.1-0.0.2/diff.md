# Comparing `tmp/pl_liblab_lotr_sdk-0.0.1.tar.gz` & `tmp/pl_liblab_lotr_sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pl_liblab_lotr_sdk-0.0.1.tar", max compression
+gzip compressed data, was "pl_liblab_lotr_sdk-0.0.2.tar", max compression
```

## Comparing `pl_liblab_lotr_sdk-0.0.1.tar` & `pl_liblab_lotr_sdk-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1044 2023-04-18 20:03:49.332932 pl_liblab_lotr_sdk-0.0.1/LICENSE
--rw-r--r--   0        0        0      638 2023-04-18 20:40:45.128909 pl_liblab_lotr_sdk-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-04-18 16:45:55.364017 pl_liblab_lotr_sdk-0.0.1/pl_liblab_lotr_sdk/__init__.py
--rw-r--r--   0        0        0     1511 2023-04-18 19:53:39.720454 pl_liblab_lotr_sdk-0.0.1/pl_liblab_lotr_sdk/api.py
--rw-r--r--   0        0        0      819 2023-04-18 19:53:53.800985 pl_liblab_lotr_sdk-0.0.1/pl_liblab_lotr_sdk/models.py
--rw-r--r--   0        0        0      401 2023-04-18 20:27:08.961088 pl_liblab_lotr_sdk-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1123 1970-01-01 00:00:00.000000 pl_liblab_lotr_sdk-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1044 2023-04-18 20:03:49.332932 pl_liblab_lotr_sdk-0.0.2/LICENSE
+-rw-r--r--   0        0        0      716 2023-04-18 20:48:49.480622 pl_liblab_lotr_sdk-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-18 16:45:55.364017 pl_liblab_lotr_sdk-0.0.2/pl_liblab_lotr_sdk/__init__.py
+-rw-r--r--   0        0        0     1511 2023-04-18 19:53:39.720454 pl_liblab_lotr_sdk-0.0.2/pl_liblab_lotr_sdk/api.py
+-rw-r--r--   0        0        0      819 2023-04-18 19:53:53.800985 pl_liblab_lotr_sdk-0.0.2/pl_liblab_lotr_sdk/models.py
+-rw-r--r--   0        0        0      401 2023-04-18 20:49:31.441702 pl_liblab_lotr_sdk-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1201 1970-01-01 00:00:00.000000 pl_liblab_lotr_sdk-0.0.2/PKG-INFO
```

### Comparing `pl_liblab_lotr_sdk-0.0.1/LICENSE` & `pl_liblab_lotr_sdk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pl_liblab_lotr_sdk-0.0.1/README.md` & `pl_liblab_lotr_sdk-0.0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -9,34 +9,34 @@
 ```
 pip install pl-liblab-lotr-sdk
 ```
 
 Use the package:
 
 ```python
-from lotr import client
+from pl_liblab_lotr_sdk.api import Client
 
-client = Client(key=<api_key>)
-client.get_movies()
+client = Client(api_key="<api_key>")
+for movie in client.get_movie():
+    print(movie.name)
 ```
 
 
 # Developing
 
 To develop his library:
+
 0. Install [Poetry](https://python-poetry.org/)
 1. Copy `.env.sample` to `.env` then add your API key.
 2. Create a virtual env `python -m venv .venv`
 3. Activate venv `source .venv/bin/activate`
 4. Install libraries `pip install -r requirements.txt`
-
-Run tests:
-```bash
-./test.sh
-```
+5. Run Tests: `./test.sh`
 
 # Release
 
+Release packages to PyPI
+
 ```python
 poetry config pypi-token pypi-YYYYYYYY
 poetry publish
 ```
```

### Comparing `pl_liblab_lotr_sdk-0.0.1/pl_liblab_lotr_sdk/api.py` & `pl_liblab_lotr_sdk-0.0.2/pl_liblab_lotr_sdk/api.py`

 * *Files identical despite different names*

### Comparing `pl_liblab_lotr_sdk-0.0.1/pl_liblab_lotr_sdk/models.py` & `pl_liblab_lotr_sdk-0.0.2/pl_liblab_lotr_sdk/models.py`

 * *Files identical despite different names*

### Comparing `pl_liblab_lotr_sdk-0.0.1/PKG-INFO` & `pl_liblab_lotr_sdk-0.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pl-liblab-lotr-sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -25,35 +25,35 @@
 ```
 pip install pl-liblab-lotr-sdk
 ```
 
 Use the package:
 
 ```python
-from lotr import client
+from pl_liblab_lotr_sdk.api import Client
 
-client = Client(key=<api_key>)
-client.get_movies()
+client = Client(api_key="<api_key>")
+for movie in client.get_movie():
+    print(movie.name)
 ```
 
 
 # Developing
 
 To develop his library:
+
 0. Install [Poetry](https://python-poetry.org/)
 1. Copy `.env.sample` to `.env` then add your API key.
 2. Create a virtual env `python -m venv .venv`
 3. Activate venv `source .venv/bin/activate`
 4. Install libraries `pip install -r requirements.txt`
-
-Run tests:
-```bash
-./test.sh
-```
+5. Run Tests: `./test.sh`
 
 # Release
 
+Release packages to PyPI
+
 ```python
 poetry config pypi-token pypi-YYYYYYYY
 poetry publish
 ```
```

