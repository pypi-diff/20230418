# Comparing `tmp/ekumenlabs_config-0.1.0.tar.gz` & `tmp/ekumenlabs_config-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ekumenlabs_config-0.1.0.tar", max compression
+gzip compressed data, was "ekumenlabs_config-0.1.1.tar", max compression
```

## Comparing `ekumenlabs_config-0.1.0.tar` & `ekumenlabs_config-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1077 2023-04-17 20:15:00.347274 ekumenlabs_config-0.1.0/LICENSE
--rw-r--r--   0        0        0      985 2023-04-18 13:09:47.711645 ekumenlabs_config-0.1.0/README.md
--rw-r--r--   0        0        0      515 2023-04-17 17:33:07.149166 ekumenlabs_config-0.1.0/ekumenlabs_config/__init__.py
--rw-r--r--   0        0        0      110 2023-04-17 16:05:00.478141 ekumenlabs_config-0.1.0/ekumenlabs_config/exceptions.py
--rw-r--r--   0        0        0     3174 2023-04-17 18:28:28.778025 ekumenlabs_config-0.1.0/ekumenlabs_config/models.py
--rw-r--r--   0        0        0      828 2023-04-18 16:05:55.156714 ekumenlabs_config-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1678 2023-04-18 16:06:16.349366 ekumenlabs_config-0.1.0/setup.py
--rw-r--r--   0        0        0     1749 2023-04-18 16:06:16.349503 ekumenlabs_config-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-18 16:17:46.886373 ekumenlabs_config-0.1.1/LICENSE
+-rw-r--r--   0        0        0      985 2023-04-18 16:17:46.886373 ekumenlabs_config-0.1.1/README.md
+-rw-r--r--   0        0        0      515 2023-04-18 16:17:46.886373 ekumenlabs_config-0.1.1/ekumenlabs_config/__init__.py
+-rw-r--r--   0        0        0      110 2023-04-18 16:17:46.886373 ekumenlabs_config-0.1.1/ekumenlabs_config/exceptions.py
+-rw-r--r--   0        0        0     3174 2023-04-18 16:17:46.886373 ekumenlabs_config-0.1.1/ekumenlabs_config/models.py
+-rw-r--r--   0        0        0      828 2023-04-18 16:17:46.886373 ekumenlabs_config-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1800 1970-01-01 00:00:00.000000 ekumenlabs_config-0.1.1/PKG-INFO
```

### Comparing `ekumenlabs_config-0.1.0/LICENSE` & `ekumenlabs_config-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ekumenlabs_config-0.1.0/README.md` & `ekumenlabs_config-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ekumenlabs_config-0.1.0/ekumenlabs_config/__init__.py` & `ekumenlabs_config-0.1.1/ekumenlabs_config/__init__.py`

 * *Files identical despite different names*

### Comparing `ekumenlabs_config-0.1.0/ekumenlabs_config/models.py` & `ekumenlabs_config-0.1.1/ekumenlabs_config/models.py`

 * *Files identical despite different names*

### Comparing `ekumenlabs_config-0.1.0/pyproject.toml` & `ekumenlabs_config-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ekumenlabs_config"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Guillermo Manzato <manzato@ekumenlabs.com>"]
 license = "MIT"
 readme = "README.md"
 
 homepage = "https://github.com/Ekumen-OS/ekumenlabs_config"
 repository = "https://github.com/Ekumen-OS/ekumenlabs_config"
```

### Comparing `ekumenlabs_config-0.1.0/PKG-INFO` & `ekumenlabs_config-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: ekumenlabs-config
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Home-page: https://github.com/Ekumen-OS/ekumenlabs_config
 License: MIT
 Keywords: configuration
 Author: Guillermo Manzato
 Author-email: manzato@ekumenlabs.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: tortoise-orm (>=0.19.2,<0.20.0)
 Project-URL: Documentation, https://github.com/Ekumen-OS/ekumenlabs_config
 Project-URL: Repository, https://github.com/Ekumen-OS/ekumenlabs_config
 Description-Content-Type: text/markdown
 
 # ekumenlabs_config
```

