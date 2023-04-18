# Comparing `tmp/bybitHTTPX-0.0.2.tar.gz` & `tmp/bybitHTTPX-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bybitHTTPX-0.0.2.tar", last modified: Tue Apr 18 06:41:13 2023, max compression
+gzip compressed data, was "bybitHTTPX-0.0.3.tar", last modified: Tue Apr 18 13:00:27 2023, max compression
```

## Comparing `bybitHTTPX-0.0.2.tar` & `bybitHTTPX-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 06:41:13.803364 bybitHTTPX-0.0.2/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-04-16 18:11:22.000000 bybitHTTPX-0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      642 2023-04-18 06:41:13.803364 bybitHTTPX-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      119 2023-04-16 18:11:22.000000 bybitHTTPX-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 06:41:13.800031 bybitHTTPX-0.0.2/bybitHTTPX/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 06:41:13.803364 bybitHTTPX-0.0.2/bybitHTTPX/bybitHTTPX.egg-info/
--rw-r--r--   0 root         (0) root         (0)      642 2023-04-18 06:41:13.000000 bybitHTTPX-0.0.2/bybitHTTPX/bybitHTTPX.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      266 2023-04-18 06:41:13.000000 bybitHTTPX-0.0.2/bybitHTTPX/bybitHTTPX.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 06:41:13.000000 bybitHTTPX-0.0.2/bybitHTTPX/bybitHTTPX.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-18 06:41:13.000000 bybitHTTPX-0.0.2/bybitHTTPX/bybitHTTPX.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 06:41:13.000000 bybitHTTPX-0.0.2/bybitHTTPX/bybitHTTPX.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-04-16 18:23:55.000000 bybitHTTPX-0.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      697 2023-04-18 06:41:13.806697 bybitHTTPX-0.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:00:27.420595 bybitHTTPX-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-04-18 12:43:40.000000 bybitHTTPX-0.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      642 2023-04-18 13:00:27.420595 bybitHTTPX-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      119 2023-04-18 12:43:40.000000 bybitHTTPX-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:00:27.413928 bybitHTTPX-0.0.3/bybitHTTPX/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:00:27.420595 bybitHTTPX-0.0.3/bybitHTTPX/bybitHTTPX.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-04-18 13:00:27.000000 bybitHTTPX-0.0.3/bybitHTTPX/bybitHTTPX.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      266 2023-04-18 13:00:27.000000 bybitHTTPX-0.0.3/bybitHTTPX/bybitHTTPX.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 13:00:27.000000 bybitHTTPX-0.0.3/bybitHTTPX/bybitHTTPX.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-18 13:00:27.000000 bybitHTTPX-0.0.3/bybitHTTPX/bybitHTTPX.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 13:00:27.000000 bybitHTTPX-0.0.3/bybitHTTPX/bybitHTTPX.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-04-18 12:43:40.000000 bybitHTTPX-0.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      697 2023-04-18 13:00:27.423928 bybitHTTPX-0.0.3/setup.cfg
```

### Comparing `bybitHTTPX-0.0.2/LICENSE` & `bybitHTTPX-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bybitHTTPX-0.0.2/PKG-INFO` & `bybitHTTPX-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bybitHTTPX
-Version: 0.0.2
+Version: 0.0.3
 Summary: a httpx wrapper for bybit API
 Home-page: https://github.com/ShaharBrandman/bybitHTTPX
 Author: Shahar Brandman
 Author-email: shaharbrandman@gmail.com
 Project-URL: Bug Tracker, https://github.com/ShaharBrandman/bybitHTTPX/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bybitHTTPX-0.0.2/bybitHTTPX/bybitHTTPX.egg-info/PKG-INFO` & `bybitHTTPX-0.0.3/bybitHTTPX/bybitHTTPX.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bybitHTTPX
-Version: 0.0.2
+Version: 0.0.3
 Summary: a httpx wrapper for bybit API
 Home-page: https://github.com/ShaharBrandman/bybitHTTPX
 Author: Shahar Brandman
 Author-email: shaharbrandman@gmail.com
 Project-URL: Bug Tracker, https://github.com/ShaharBrandman/bybitHTTPX/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bybitHTTPX-0.0.2/setup.cfg` & `bybitHTTPX-0.0.3/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bybitHTTPX
-version = 0.0.2
+version = 0.0.3
 author = Shahar Brandman
 author_email = shaharbrandman@gmail.com
 description = a httpx wrapper for bybit API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ShaharBrandman/bybitHTTPX
 project_urls =
```

