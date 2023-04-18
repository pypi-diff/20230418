# Comparing `tmp/basicnanoclient-0.0.4.tar.gz` & `tmp/basicnanoclient-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basicnanoclient-0.0.4.tar", last modified: Tue Apr 18 03:43:59 2023, max compression
+gzip compressed data, was "basicnanoclient-0.0.5.tar", last modified: Tue Apr 18 04:09:57 2023, max compression
```

## Comparing `basicnanoclient-0.0.4.tar` & `basicnanoclient-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-18 03:43:59.174596 basicnanoclient-0.0.4/
--rw-r--r--   0 nate       (501) staff       (20)     1211 2023-04-18 02:36:25.000000 basicnanoclient-0.0.4/LICENSE
--rw-r--r--   0 nate       (501) staff       (20)     2762 2023-04-18 03:43:59.174480 basicnanoclient-0.0.4/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)      844 2023-04-18 03:14:16.000000 basicnanoclient-0.0.4/README.md
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-18 03:43:59.174331 basicnanoclient-0.0.4/basicnanoclient.egg-info/
--rw-r--r--   0 nate       (501) staff       (20)     2762 2023-04-18 03:43:59.000000 basicnanoclient-0.0.4/basicnanoclient.egg-info/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)      235 2023-04-18 03:43:59.000000 basicnanoclient-0.0.4/basicnanoclient.egg-info/SOURCES.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-18 03:43:59.000000 basicnanoclient-0.0.4/basicnanoclient.egg-info/dependency_links.txt
--rw-r--r--   0 nate       (501) staff       (20)       99 2023-04-18 03:43:59.000000 basicnanoclient-0.0.4/basicnanoclient.egg-info/requires.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-18 03:43:59.000000 basicnanoclient-0.0.4/basicnanoclient.egg-info/top_level.txt
--rw-r--r--   0 nate       (501) staff       (20)      728 2023-04-18 03:43:04.000000 basicnanoclient-0.0.4/pyproject.toml
--rw-r--r--   0 nate       (501) staff       (20)       38 2023-04-18 03:43:59.174629 basicnanoclient-0.0.4/setup.cfg
--rw-r--r--   0 nate       (501) staff       (20)      943 2023-04-18 03:39:55.000000 basicnanoclient-0.0.4/setup.py
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-18 04:09:57.226399 basicnanoclient-0.0.5/
+-rw-r--r--   0 nate       (501) staff       (20)     1211 2023-04-18 02:36:25.000000 basicnanoclient-0.0.5/LICENSE
+-rw-r--r--   0 nate       (501) staff       (20)     2762 2023-04-18 04:09:57.226282 basicnanoclient-0.0.5/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)      844 2023-04-18 03:14:16.000000 basicnanoclient-0.0.5/README.md
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-18 04:09:57.226149 basicnanoclient-0.0.5/basicnanoclient.egg-info/
+-rw-r--r--   0 nate       (501) staff       (20)     2762 2023-04-18 04:09:57.000000 basicnanoclient-0.0.5/basicnanoclient.egg-info/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)      235 2023-04-18 04:09:57.000000 basicnanoclient-0.0.5/basicnanoclient.egg-info/SOURCES.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-18 04:09:57.000000 basicnanoclient-0.0.5/basicnanoclient.egg-info/dependency_links.txt
+-rw-r--r--   0 nate       (501) staff       (20)       60 2023-04-18 04:09:57.000000 basicnanoclient-0.0.5/basicnanoclient.egg-info/requires.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-18 04:09:57.000000 basicnanoclient-0.0.5/basicnanoclient.egg-info/top_level.txt
+-rw-r--r--   0 nate       (501) staff       (20)      675 2023-04-18 04:06:33.000000 basicnanoclient-0.0.5/pyproject.toml
+-rw-r--r--   0 nate       (501) staff       (20)       38 2023-04-18 04:09:57.226429 basicnanoclient-0.0.5/setup.cfg
+-rw-r--r--   0 nate       (501) staff       (20)      943 2023-04-18 04:06:28.000000 basicnanoclient-0.0.5/setup.py
```

### Comparing `basicnanoclient-0.0.4/LICENSE` & `basicnanoclient-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `basicnanoclient-0.0.4/PKG-INFO` & `basicnanoclient-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basicnanoclient
-Version: 0.0.4
+Version: 0.0.5
 Summary: Nano RPC python client
 Home-page: https://github.com/nanoswap/basicnanoclient
 Author: Nathaniel Schultz
 Author-email: Nathaniel Schultz <nate@nanoswap.finance>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
```

### Comparing `basicnanoclient-0.0.4/README.md` & `basicnanoclient-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `basicnanoclient-0.0.4/basicnanoclient.egg-info/PKG-INFO` & `basicnanoclient-0.0.5/basicnanoclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basicnanoclient
-Version: 0.0.4
+Version: 0.0.5
 Summary: Nano RPC python client
 Home-page: https://github.com/nanoswap/basicnanoclient
 Author: Nathaniel Schultz
 Author-email: Nathaniel Schultz <nate@nanoswap.finance>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
```

### Comparing `basicnanoclient-0.0.4/pyproject.toml` & `basicnanoclient-0.0.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,27 +2,25 @@
 source = ["basicnanoclient", "*/site-packages"]
 
 [tool.coverage.report]
 show_missing = true
 
 [project]
 name = "basicnanoclient"
-version = "0.0.4"
+version = "0.0.5"
 description = "Nano RPC python client"
 urls = {'Bug Tracker' = 'https://github.com/nanoswap/basicnanoclient/issues'}
 classifiers = [
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: The Unlicense (Unlicense)'
 ]
 authors = [{'name' = 'Nathaniel Schultz', 'email' = 'nate@nanoswap.finance'}]
 requires-python = '>=3.11'
 readme = 'README.md'
 license = {'file' = 'LICENSE'}
 dependencies = [
     "requests",
     "setuptools",
-    "jinja2==2.11",
-    "markupsafe==1.1.1",
     "mkdocs",
-    "mkdocstrings>=0.16.1",
+    "mkdocstrings",
     "mkdocstrings-python"
 ]
```

### Comparing `basicnanoclient-0.0.4/setup.py` & `basicnanoclient-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     """Convert README.md to a string."""
     with open(filename, "r", encoding="utf-8") as f:
         return f.read()
 
 
 setup(
     name="basicnanoclient",
-    version="0.0.4",
+    version="0.0.5",
     author="Nathaniel Schultz",
     author_email="nate@nanoswap.finance",
     description="Nano Cryptocurrency RPC Client",
     long_description=load_long_description("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/nanoswap/basicnanoclient",
     project_urls={
```

