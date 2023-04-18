# Comparing `tmp/gitfluencer-0.1.1.tar.gz` & `tmp/gitfluencer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitfluencer-0.1.1.tar", last modified: Tue Apr 18 08:27:42 2023, max compression
+gzip compressed data, was "gitfluencer-0.1.2.tar", last modified: Tue Apr 18 08:32:11 2023, max compression
```

## Comparing `gitfluencer-0.1.1.tar` & `gitfluencer-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-04-18 08:27:42.101518 gitfluencer-0.1.1/
--rw-r--r--   0 joel      (1000) joel      (1000)      755 2023-04-18 08:27:42.101518 gitfluencer-0.1.1/PKG-INFO
--rw-r--r--   0 joel      (1000) joel      (1000)      951 2023-04-18 07:59:49.000000 gitfluencer-0.1.1/README.md
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-04-18 08:27:42.100519 gitfluencer-0.1.1/gitfluencer/
--rw-r--r--   0 joel      (1000) joel      (1000)        0 2023-04-18 08:01:35.000000 gitfluencer-0.1.1/gitfluencer/__init__.py
--rw-r--r--   0 joel      (1000) joel      (1000)     2443 2023-04-18 08:25:40.000000 gitfluencer-0.1.1/gitfluencer/app.py
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-04-18 08:27:42.101518 gitfluencer-0.1.1/gitfluencer.egg-info/
--rw-r--r--   0 joel      (1000) joel      (1000)      755 2023-04-18 08:27:42.000000 gitfluencer-0.1.1/gitfluencer.egg-info/PKG-INFO
--rw-r--r--   0 joel      (1000) joel      (1000)      273 2023-04-18 08:27:42.000000 gitfluencer-0.1.1/gitfluencer.egg-info/SOURCES.txt
--rw-r--r--   0 joel      (1000) joel      (1000)        1 2023-04-18 08:27:42.000000 gitfluencer-0.1.1/gitfluencer.egg-info/dependency_links.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       53 2023-04-18 08:27:42.000000 gitfluencer-0.1.1/gitfluencer.egg-info/entry_points.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       30 2023-04-18 08:27:42.000000 gitfluencer-0.1.1/gitfluencer.egg-info/requires.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       12 2023-04-18 08:27:42.000000 gitfluencer-0.1.1/gitfluencer.egg-info/top_level.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       38 2023-04-18 08:27:42.101518 gitfluencer-0.1.1/setup.cfg
--rw-r--r--   0 joel      (1000) joel      (1000)     1072 2023-04-18 08:27:06.000000 gitfluencer-0.1.1/setup.py
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-04-18 08:32:11.054740 gitfluencer-0.1.2/
+-rw-r--r--   0 joel      (1000) joel      (1000)      755 2023-04-18 08:32:11.054740 gitfluencer-0.1.2/PKG-INFO
+-rw-r--r--   0 joel      (1000) joel      (1000)      951 2023-04-18 07:59:49.000000 gitfluencer-0.1.2/README.md
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-04-18 08:32:11.053740 gitfluencer-0.1.2/gitfluencer/
+-rw-r--r--   0 joel      (1000) joel      (1000)        0 2023-04-18 08:01:35.000000 gitfluencer-0.1.2/gitfluencer/__init__.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     2368 2023-04-18 08:31:48.000000 gitfluencer-0.1.2/gitfluencer/app.py
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-04-18 08:32:11.054740 gitfluencer-0.1.2/gitfluencer.egg-info/
+-rw-r--r--   0 joel      (1000) joel      (1000)      755 2023-04-18 08:32:11.000000 gitfluencer-0.1.2/gitfluencer.egg-info/PKG-INFO
+-rw-r--r--   0 joel      (1000) joel      (1000)      273 2023-04-18 08:32:11.000000 gitfluencer-0.1.2/gitfluencer.egg-info/SOURCES.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)        1 2023-04-18 08:32:11.000000 gitfluencer-0.1.2/gitfluencer.egg-info/dependency_links.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       53 2023-04-18 08:32:11.000000 gitfluencer-0.1.2/gitfluencer.egg-info/entry_points.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       23 2023-04-18 08:32:11.000000 gitfluencer-0.1.2/gitfluencer.egg-info/requires.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       12 2023-04-18 08:32:11.000000 gitfluencer-0.1.2/gitfluencer.egg-info/top_level.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       38 2023-04-18 08:32:11.054740 gitfluencer-0.1.2/setup.cfg
+-rw-r--r--   0 joel      (1000) joel      (1000)     1065 2023-04-18 08:31:53.000000 gitfluencer-0.1.2/setup.py
```

### Comparing `gitfluencer-0.1.1/PKG-INFO` & `gitfluencer-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitfluencer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Utility tool for interacting with the GitHub platform
 Home-page: https://github.com/jjoeldaniel/gitfluencer
 Author: jjoeldaniel
 Author-email: joeldanielrico@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `gitfluencer-0.1.1/README.md` & `gitfluencer-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gitfluencer-0.1.1/gitfluencer/app.py` & `gitfluencer-0.1.2/gitfluencer/app.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from github import Github
-from dotenv import load_dotenv
 from rich import print
 from rich.console import Console
 from rich.table import Table
 from rich.prompt import Prompt, Confirm
 import os
 import requests
 
-# Load environment variables
-load_dotenv()
-
 # Get API token from environment variable or prompt for input
 api_token = os.getenv("API_TOKEN")
 if not api_token:
     api_token = input("Please enter your GitHub API token: ")
 
 # Store API token as environment variable
 os.environ["API_TOKEN"] = api_token
```

### Comparing `gitfluencer-0.1.1/gitfluencer.egg-info/PKG-INFO` & `gitfluencer-0.1.2/gitfluencer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitfluencer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Utility tool for interacting with the GitHub platform
 Home-page: https://github.com/jjoeldaniel/gitfluencer
 Author: jjoeldaniel
 Author-email: joeldanielrico@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `gitfluencer-0.1.1/setup.py` & `gitfluencer-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gitfluencer',
-    version='0.1.1',
+    version='0.1.2',
     description='Utility tool for interacting with the GitHub platform',
     author='jjoeldaniel',
     author_email='joeldanielrico@gmail.com',
     url='https://github.com/jjoeldaniel/gitfluencer',
     packages=find_packages(),
     install_requires=[
-        'github3.py',
-        'python-dotenv',
+        'PyGithub',
+        'Requests',
         'rich',
     ],
     entry_points={
         'console_scripts': [
             'gitfluencer=gitfluencer.app:main',
         ],
     },
```

