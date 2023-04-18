# Comparing `tmp/gitfluencer-0.1.2.tar.gz` & `tmp/gitfluencer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitfluencer-0.1.2.tar", last modified: Tue Apr 18 08:32:11 2023, max compression
+gzip compressed data, was "gitfluencer-0.1.3.tar", last modified: Tue Apr 18 08:56:41 2023, max compression
```

## Comparing `gitfluencer-0.1.2.tar` & `gitfluencer-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-04-18 08:32:11.054740 gitfluencer-0.1.2/
--rw-r--r--   0 joel      (1000) joel      (1000)      755 2023-04-18 08:32:11.054740 gitfluencer-0.1.2/PKG-INFO
--rw-r--r--   0 joel      (1000) joel      (1000)      951 2023-04-18 07:59:49.000000 gitfluencer-0.1.2/README.md
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-04-18 08:32:11.053740 gitfluencer-0.1.2/gitfluencer/
--rw-r--r--   0 joel      (1000) joel      (1000)        0 2023-04-18 08:01:35.000000 gitfluencer-0.1.2/gitfluencer/__init__.py
--rw-r--r--   0 joel      (1000) joel      (1000)     2368 2023-04-18 08:31:48.000000 gitfluencer-0.1.2/gitfluencer/app.py
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-04-18 08:32:11.054740 gitfluencer-0.1.2/gitfluencer.egg-info/
--rw-r--r--   0 joel      (1000) joel      (1000)      755 2023-04-18 08:32:11.000000 gitfluencer-0.1.2/gitfluencer.egg-info/PKG-INFO
--rw-r--r--   0 joel      (1000) joel      (1000)      273 2023-04-18 08:32:11.000000 gitfluencer-0.1.2/gitfluencer.egg-info/SOURCES.txt
--rw-r--r--   0 joel      (1000) joel      (1000)        1 2023-04-18 08:32:11.000000 gitfluencer-0.1.2/gitfluencer.egg-info/dependency_links.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       53 2023-04-18 08:32:11.000000 gitfluencer-0.1.2/gitfluencer.egg-info/entry_points.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       23 2023-04-18 08:32:11.000000 gitfluencer-0.1.2/gitfluencer.egg-info/requires.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       12 2023-04-18 08:32:11.000000 gitfluencer-0.1.2/gitfluencer.egg-info/top_level.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       38 2023-04-18 08:32:11.054740 gitfluencer-0.1.2/setup.cfg
--rw-r--r--   0 joel      (1000) joel      (1000)     1065 2023-04-18 08:31:53.000000 gitfluencer-0.1.2/setup.py
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-04-18 08:56:41.042553 gitfluencer-0.1.3/
+-rw-r--r--   0 joel      (1000) joel      (1000)      755 2023-04-18 08:56:41.042553 gitfluencer-0.1.3/PKG-INFO
+-rw-r--r--   0 joel      (1000) joel      (1000)      951 2023-04-18 07:59:49.000000 gitfluencer-0.1.3/README.md
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-04-18 08:56:41.042553 gitfluencer-0.1.3/gitfluencer/
+-rw-r--r--   0 joel      (1000) joel      (1000)        0 2023-04-18 08:01:35.000000 gitfluencer-0.1.3/gitfluencer/__init__.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     2476 2023-04-18 08:55:35.000000 gitfluencer-0.1.3/gitfluencer/app.py
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-04-18 08:56:41.042553 gitfluencer-0.1.3/gitfluencer.egg-info/
+-rw-r--r--   0 joel      (1000) joel      (1000)      755 2023-04-18 08:56:41.000000 gitfluencer-0.1.3/gitfluencer.egg-info/PKG-INFO
+-rw-r--r--   0 joel      (1000) joel      (1000)      273 2023-04-18 08:56:41.000000 gitfluencer-0.1.3/gitfluencer.egg-info/SOURCES.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)        1 2023-04-18 08:56:41.000000 gitfluencer-0.1.3/gitfluencer.egg-info/dependency_links.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       53 2023-04-18 08:56:41.000000 gitfluencer-0.1.3/gitfluencer.egg-info/entry_points.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       23 2023-04-18 08:56:41.000000 gitfluencer-0.1.3/gitfluencer.egg-info/requires.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       12 2023-04-18 08:56:41.000000 gitfluencer-0.1.3/gitfluencer.egg-info/top_level.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       38 2023-04-18 08:56:41.042553 gitfluencer-0.1.3/setup.cfg
+-rw-r--r--   0 joel      (1000) joel      (1000)     1065 2023-04-18 08:56:18.000000 gitfluencer-0.1.3/setup.py
```

### Comparing `gitfluencer-0.1.2/PKG-INFO` & `gitfluencer-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitfluencer
-Version: 0.1.2
+Version: 0.1.3
 Summary: Utility tool for interacting with the GitHub platform
 Home-page: https://github.com/jjoeldaniel/gitfluencer
 Author: jjoeldaniel
 Author-email: joeldanielrico@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `gitfluencer-0.1.2/README.md` & `gitfluencer-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `gitfluencer-0.1.2/gitfluencer/app.py` & `gitfluencer-0.1.3/gitfluencer/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 from rich.prompt import Prompt, Confirm
 import os
 import requests
 
 # Get API token from environment variable or prompt for input
 api_token = os.getenv("API_TOKEN")
 if not api_token:
-    api_token = input("Please enter your GitHub API token: ")
+    api_token = Prompt.ask(
+            "Please enter your GitHub API token: ",
+            password=True,
+            show_default=False,
+            show_choices=True)
 
 # Store API token as environment variable
 os.environ["API_TOKEN"] = api_token
 
 # Create API object from token
 git = Github(api_token)
 to_be_unfollowed = list()
```

### Comparing `gitfluencer-0.1.2/gitfluencer.egg-info/PKG-INFO` & `gitfluencer-0.1.3/gitfluencer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitfluencer
-Version: 0.1.2
+Version: 0.1.3
 Summary: Utility tool for interacting with the GitHub platform
 Home-page: https://github.com/jjoeldaniel/gitfluencer
 Author: jjoeldaniel
 Author-email: joeldanielrico@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `gitfluencer-0.1.2/setup.py` & `gitfluencer-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gitfluencer',
-    version='0.1.2',
+    version='0.1.3',
     description='Utility tool for interacting with the GitHub platform',
     author='jjoeldaniel',
     author_email='joeldanielrico@gmail.com',
     url='https://github.com/jjoeldaniel/gitfluencer',
     packages=find_packages(),
     install_requires=[
         'PyGithub',
```

