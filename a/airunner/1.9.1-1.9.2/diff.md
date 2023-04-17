# Comparing `tmp/airunner-1.9.1.tar.gz` & `tmp/airunner-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airunner-1.9.1.tar", last modified: Mon Apr 17 23:20:49 2023, max compression
+gzip compressed data, was "airunner-1.9.2.tar", last modified: Mon Apr 17 23:55:05 2023, max compression
```

## Comparing `airunner-1.9.1.tar` & `airunner-1.9.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:20:49.084199 airunner-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-17 23:20:37.000000 airunner-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-04-17 23:20:49.084199 airunner-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-17 23:20:37.000000 airunner-1.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 23:20:49.084199 airunner-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-17 23:20:37.000000 airunner-1.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:20:49.084199 airunner-1.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:20:49.084199 airunner-1.9.1/src/airunner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 23:20:37.000000 airunner-1.9.1/src/airunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-17 23:20:37.000000 airunner-1.9.1/src/airunner/balloon.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-17 23:20:37.000000 airunner-1.9.1/src/airunner/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-17 23:20:37.000000 airunner-1.9.1/src/airunner/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-17 23:20:37.000000 airunner-1.9.1/src/airunner/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-17 23:20:37.000000 airunner-1.9.1/src/airunner/history.py
--rw-r--r--   0 runner    (1001) docker     (123)    64664 2023-04-17 23:20:37.000000 airunner-1.9.1/src/airunner/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    34662 2023-04-17 23:20:37.000000 airunner-1.9.1/src/airunner/qtcanvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-04-17 23:20:37.000000 airunner-1.9.1/src/airunner/runai_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-17 23:20:37.000000 airunner-1.9.1/src/airunner/settingsmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-04-17 23:20:38.000000 airunner-1.9.1/src/airunner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:20:49.084199 airunner-1.9.1/src/airunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-04-17 23:20:49.000000 airunner-1.9.1/src/airunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-17 23:20:49.000000 airunner-1.9.1/src/airunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 23:20:49.000000 airunner-1.9.1/src/airunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-17 23:20:49.000000 airunner-1.9.1/src/airunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 23:20:49.000000 airunner-1.9.1/src/airunner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:55:05.946614 airunner-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-17 23:54:54.000000 airunner-1.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-04-17 23:55:05.946614 airunner-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-17 23:54:54.000000 airunner-1.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 23:55:05.946614 airunner-1.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-17 23:54:54.000000 airunner-1.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:55:05.942614 airunner-1.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:55:05.946614 airunner-1.9.2/src/airunner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 23:54:54.000000 airunner-1.9.2/src/airunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-17 23:54:54.000000 airunner-1.9.2/src/airunner/balloon.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-17 23:54:54.000000 airunner-1.9.2/src/airunner/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-17 23:54:54.000000 airunner-1.9.2/src/airunner/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-17 23:54:54.000000 airunner-1.9.2/src/airunner/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-17 23:54:54.000000 airunner-1.9.2/src/airunner/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64664 2023-04-17 23:54:54.000000 airunner-1.9.2/src/airunner/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34662 2023-04-17 23:54:54.000000 airunner-1.9.2/src/airunner/qtcanvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-04-17 23:54:54.000000 airunner-1.9.2/src/airunner/runai_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-17 23:54:54.000000 airunner-1.9.2/src/airunner/settingsmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-04-17 23:54:54.000000 airunner-1.9.2/src/airunner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:55:05.946614 airunner-1.9.2/src/airunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-04-17 23:55:05.000000 airunner-1.9.2/src/airunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-17 23:55:05.000000 airunner-1.9.2/src/airunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 23:55:05.000000 airunner-1.9.2/src/airunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-17 23:55:05.000000 airunner-1.9.2/src/airunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 23:55:05.000000 airunner-1.9.2/src/airunner.egg-info/top_level.txt
```

### Comparing `airunner-1.9.1/LICENSE` & `airunner-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `airunner-1.9.1/PKG-INFO` & `airunner-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airunner
-Version: 1.9.1
+Version: 1.9.2
 Summary: A Stable Diffusion GUI
 Home-page: https://github.com/Capsize-Games/airunner
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
```

### Comparing `airunner-1.9.1/README.md` & `airunner-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `airunner-1.9.1/setup.py` & `airunner-1.9.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='airunner',
-    version="1.9.1",
+    version="1.9.2",
     author="Capsize LLC",
     description="A Stable Diffusion GUI",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="ai, chatbot, chat, ai",
     license="AGPL-3.0",
     author_email="contact@capsize.gg",
     url="https://github.com/Capsize-Games/airunner",
     package_dir={"": "src"},
     packages=find_packages("src"),
     python_requires=">=3.10.0",
     install_requires=[
-        "aihandler==1.9.5",
+        "aihandler==1.9.6",
     ]
 )
```

### Comparing `airunner-1.9.1/src/airunner/balloon.py` & `airunner-1.9.2/src/airunner/balloon.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.1/src/airunner/extensions.py` & `airunner-1.9.2/src/airunner/extensions.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.1/src/airunner/filters.py` & `airunner-1.9.2/src/airunner/filters.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.1/src/airunner/main.py` & `airunner-1.9.2/src/airunner/main.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.1/src/airunner/qtcanvas.py` & `airunner-1.9.2/src/airunner/qtcanvas.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.1/src/airunner/runai_client.py` & `airunner-1.9.2/src/airunner/runai_client.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.1/src/airunner/settingsmanager.py` & `airunner-1.9.2/src/airunner/settingsmanager.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.1/src/airunner/utils.py` & `airunner-1.9.2/src/airunner/utils.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.1/src/airunner.egg-info/PKG-INFO` & `airunner-1.9.2/src/airunner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airunner
-Version: 1.9.1
+Version: 1.9.2
 Summary: A Stable Diffusion GUI
 Home-page: https://github.com/Capsize-Games/airunner
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
```

