# Comparing `tmp/acr122u-websocket-1.1.2.tar.gz` & `tmp/acr122u-websocket-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acr122u-websocket-1.1.2.tar", last modified: Tue Apr 18 14:59:20 2023, max compression
+gzip compressed data, was "acr122u-websocket-1.1.3.tar", last modified: Tue Apr 18 15:01:54 2023, max compression
```

## Comparing `acr122u-websocket-1.1.2.tar` & `acr122u-websocket-1.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:59:20.856946 acr122u-websocket-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-18 14:59:05.000000 acr122u-websocket-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-18 14:59:20.856946 acr122u-websocket-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-18 14:59:05.000000 acr122u-websocket-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:59:20.856946 acr122u-websocket-1.1.2/acr122u_websocket/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 14:59:05.000000 acr122u-websocket-1.1.2/acr122u_websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-18 14:59:05.000000 acr122u-websocket-1.1.2/acr122u_websocket/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-18 14:59:05.000000 acr122u-websocket-1.1.2/acr122u_websocket/my_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-18 14:59:05.000000 acr122u-websocket-1.1.2/acr122u_websocket/reader_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:59:20.856946 acr122u-websocket-1.1.2/acr122u_websocket/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-18 14:59:05.000000 acr122u-websocket-1.1.2/acr122u_websocket/templates/test.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:59:20.856946 acr122u-websocket-1.1.2/acr122u_websocket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-18 14:59:20.000000 acr122u-websocket-1.1.2/acr122u_websocket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-18 14:59:20.000000 acr122u-websocket-1.1.2/acr122u_websocket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:59:20.000000 acr122u-websocket-1.1.2/acr122u_websocket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-18 14:59:20.000000 acr122u-websocket-1.1.2/acr122u_websocket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 14:59:20.000000 acr122u-websocket-1.1.2/acr122u_websocket.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-18 14:59:05.000000 acr122u-websocket-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 14:59:20.856946 acr122u-websocket-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:01:54.243389 acr122u-websocket-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-18 15:01:45.000000 acr122u-websocket-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-18 15:01:54.243389 acr122u-websocket-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-18 15:01:45.000000 acr122u-websocket-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:01:54.243389 acr122u-websocket-1.1.3/acr122u_websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 15:01:45.000000 acr122u-websocket-1.1.3/acr122u_websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-18 15:01:45.000000 acr122u-websocket-1.1.3/acr122u_websocket/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-18 15:01:45.000000 acr122u-websocket-1.1.3/acr122u_websocket/my_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-18 15:01:45.000000 acr122u-websocket-1.1.3/acr122u_websocket/reader_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:01:54.243389 acr122u-websocket-1.1.3/acr122u_websocket/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-18 15:01:45.000000 acr122u-websocket-1.1.3/acr122u_websocket/templates/test.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:01:54.243389 acr122u-websocket-1.1.3/acr122u_websocket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-18 15:01:54.000000 acr122u-websocket-1.1.3/acr122u_websocket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-18 15:01:54.000000 acr122u-websocket-1.1.3/acr122u_websocket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:01:54.000000 acr122u-websocket-1.1.3/acr122u_websocket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-18 15:01:54.000000 acr122u-websocket-1.1.3/acr122u_websocket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 15:01:54.000000 acr122u-websocket-1.1.3/acr122u_websocket.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-18 15:01:45.000000 acr122u-websocket-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 15:01:54.243389 acr122u-websocket-1.1.3/setup.cfg
```

### Comparing `acr122u-websocket-1.1.2/LICENSE` & `acr122u-websocket-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `acr122u-websocket-1.1.2/PKG-INFO` & `acr122u-websocket-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acr122u-websocket
-Version: 1.1.2
+Version: 1.1.3
 Summary: A webserver that connects to a acr122u and exposes it over websocket
 Author-email: Robert van Dijk <contact@robertvandijk.nl>
 Project-URL: Homepage, https://github.com/robertdijk/acr122u-websocket
 Keywords: nfc,acr,acr122u,websocket,web
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `acr122u-websocket-1.1.2/README.md` & `acr122u-websocket-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `acr122u-websocket-1.1.2/acr122u_websocket/app.py` & `acr122u-websocket-1.1.3/acr122u_websocket/app.py`

 * *Files identical despite different names*

### Comparing `acr122u-websocket-1.1.2/acr122u_websocket/my_reader.py` & `acr122u-websocket-1.1.3/acr122u_websocket/my_reader.py`

 * *Files identical despite different names*

### Comparing `acr122u-websocket-1.1.2/acr122u_websocket/reader_helpers.py` & `acr122u-websocket-1.1.3/acr122u_websocket/reader_helpers.py`

 * *Files identical despite different names*

### Comparing `acr122u-websocket-1.1.2/acr122u_websocket/templates/test.html` & `acr122u-websocket-1.1.3/acr122u_websocket/templates/test.html`

 * *Files identical despite different names*

### Comparing `acr122u-websocket-1.1.2/acr122u_websocket.egg-info/PKG-INFO` & `acr122u-websocket-1.1.3/acr122u_websocket.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acr122u-websocket
-Version: 1.1.2
+Version: 1.1.3
 Summary: A webserver that connects to a acr122u and exposes it over websocket
 Author-email: Robert van Dijk <contact@robertvandijk.nl>
 Project-URL: Homepage, https://github.com/robertdijk/acr122u-websocket
 Keywords: nfc,acr,acr122u,websocket,web
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `acr122u-websocket-1.1.2/pyproject.toml` & `acr122u-websocket-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "acr122u-websocket"
-version = "1.1.2"
+version = "1.1.3"
 description = "A webserver that connects to a acr122u and exposes it over websocket"
 readme = "README.md"
 authors = [{ name = "Robert van Dijk", email = "contact@robertvandijk.nl" }]
 license = { file = "pb" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
@@ -35,15 +35,15 @@
     "black",
 ]
 
 [project.urls]
 Homepage = "https://github.com/robertdijk/acr122u-websocket"
 
 [tool.bumpver]
-current_version = "1.1.2"
+current_version = "1.1.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

