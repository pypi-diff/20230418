# Comparing `tmp/speedtab-0.1.2.3.tar.gz` & `tmp/speedtab-0.1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtab-0.1.2.3.tar", max compression
+gzip compressed data, was "speedtab-0.1.2.4.tar", max compression
```

## Comparing `speedtab-0.1.2.3.tar` & `speedtab-0.1.2.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      567 2023-04-18 16:09:55.741561 speedtab-0.1.2.3/pyproject.toml
--rw-r--r--   0        0        0      352 2022-09-07 08:00:08.177672 speedtab-0.1.2.3/speedtab/__init__.py
--rw-r--r--   0        0        0    35875 2023-04-18 16:08:09.813649 speedtab-0.1.2.3/speedtab/client.py
--rw-r--r--   0        0        0     5857 2022-10-11 09:11:17.745858 speedtab-0.1.2.3/speedtab/enums.py
--rw-r--r--   0        0        0     1744 2022-08-23 18:18:16.848628 speedtab-0.1.2.3/speedtab/formats.py
--rw-r--r--   0        0        0      783 2023-04-18 16:10:25.828675 speedtab-0.1.2.3/setup.py
--rw-r--r--   0        0        0      808 2023-04-18 16:10:25.828675 speedtab-0.1.2.3/PKG-INFO
+-rw-r--r--   0        0        0      567 2023-04-18 16:11:48.088583 speedtab-0.1.2.4/pyproject.toml
+-rw-r--r--   0        0        0      352 2022-09-07 08:00:08.177672 speedtab-0.1.2.4/speedtab/__init__.py
+-rw-r--r--   0        0        0    35875 2023-04-18 16:08:09.813649 speedtab-0.1.2.4/speedtab/client.py
+-rw-r--r--   0        0        0     5857 2022-10-11 09:11:17.745858 speedtab-0.1.2.4/speedtab/enums.py
+-rw-r--r--   0        0        0     1744 2022-08-23 18:18:16.848628 speedtab-0.1.2.4/speedtab/formats.py
+-rw-r--r--   0        0        0      783 2023-04-18 16:11:56.243762 speedtab-0.1.2.4/setup.py
+-rw-r--r--   0        0        0      808 2023-04-18 16:11:56.243762 speedtab-0.1.2.4/PKG-INFO
```

### Comparing `speedtab-0.1.2.3/pyproject.toml` & `speedtab-0.1.2.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "speedtab"
-version = "0.1.2.3"
+version = "0.1.2.4"
 description = "Convenient wrapper for working with Google Spreadsheets"
 authors = ["Bogdan Gergel <bogger147@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/BoggerSancho/SpeedTab-beta"
 repository = "https://github.com/BoggerSancho/SpeedTab-beta"
 
 [tool.poetry.dependencies]
```

### Comparing `speedtab-0.1.2.3/speedtab/client.py` & `speedtab-0.1.2.4/speedtab/client.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.2.3/speedtab/enums.py` & `speedtab-0.1.2.4/speedtab/enums.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.2.3/speedtab/formats.py` & `speedtab-0.1.2.4/speedtab/formats.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.2.3/setup.py` & `speedtab-0.1.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['google-api-python-client>=2.58.0,<3.0.0',
  'google-auth-httplib2>=0.1.0,<0.2.0',
  'google-auth-oauthlib>=0.5.2,<0.6.0']
 
 setup_kwargs = {
     'name': 'speedtab',
-    'version': '0.1.2.3',
+    'version': '0.1.2.4',
     'description': 'Convenient wrapper for working with Google Spreadsheets',
     'long_description': None,
     'author': 'Bogdan Gergel',
     'author_email': 'bogger147@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/BoggerSancho/SpeedTab-beta',
```

### Comparing `speedtab-0.1.2.3/PKG-INFO` & `speedtab-0.1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtab
-Version: 0.1.2.3
+Version: 0.1.2.4
 Summary: Convenient wrapper for working with Google Spreadsheets
 Home-page: https://github.com/BoggerSancho/SpeedTab-beta
 License: MIT
 Author: Bogdan Gergel
 Author-email: bogger147@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

