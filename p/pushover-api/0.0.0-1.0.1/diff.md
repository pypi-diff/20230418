# Comparing `tmp/pushover_api-0.0.0.tar.gz` & `tmp/pushover_api-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pushover_api-0.0.0.tar", max compression
+gzip compressed data, was "pushover_api-1.0.1.tar", max compression
```

## Comparing `pushover_api-0.0.0.tar` & `pushover_api-1.0.1.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0      205 2023-04-18 15:26:22.120818 pushover_api-0.0.0/README.md
--rw-r--r--   0        0        0        0 2023-04-18 15:26:22.120818 pushover_api-0.0.0/pushover/__init__.py
--rw-r--r--   0        0        0      357 2023-04-18 15:26:22.120818 pushover_api-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      627 1970-01-01 00:00:00.000000 pushover_api-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      205 2023-04-18 16:32:53.525293 pushover_api-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-18 16:32:53.525293 pushover_api-1.0.1/pushover/__init__.py
+-rw-r--r--   0        0        0      656 2023-04-18 16:32:53.525293 pushover_api-1.0.1/pushover/client.py
+-rw-r--r--   0        0        0      521 2023-04-18 16:32:53.525293 pushover_api-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      674 1970-01-01 00:00:00.000000 pushover_api-1.0.1/PKG-INFO
```

### Comparing `pushover_api-0.0.0/PKG-INFO` & `pushover_api-1.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: pushover-api
-Version: 0.0.0
+Version: 1.0.1
 Summary: 
 Author: Elvir Muslic
 Author-email: elvirmuslic.dev@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: httpx[http2] (>=0.24.0,<0.25.0)
 Requires-Dist: pre-commit (>=3.2.2,<4.0.0)
 Requires-Dist: pytest (>=7.3.1,<8.0.0)
 Description-Content-Type: text/markdown
 
 # pushover
 Unofficial API for pushover
```

