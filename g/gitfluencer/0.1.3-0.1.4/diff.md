# Comparing `tmp/gitfluencer-0.1.3.tar.gz` & `tmp/gitfluencer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitfluencer-0.1.3.tar", last modified: Tue Apr 18 08:56:41 2023, max compression
+gzip compressed data, was "gitfluencer-0.1.4.tar", last modified: Tue Apr 18 09:33:48 2023, max compression
```

## Comparing `gitfluencer-0.1.3.tar` & `gitfluencer-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-04-18 08:56:41.042553 gitfluencer-0.1.3/
--rw-r--r--   0 joel      (1000) joel      (1000)      755 2023-04-18 08:56:41.042553 gitfluencer-0.1.3/PKG-INFO
--rw-r--r--   0 joel      (1000) joel      (1000)      951 2023-04-18 07:59:49.000000 gitfluencer-0.1.3/README.md
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-04-18 08:56:41.042553 gitfluencer-0.1.3/gitfluencer/
--rw-r--r--   0 joel      (1000) joel      (1000)        0 2023-04-18 08:01:35.000000 gitfluencer-0.1.3/gitfluencer/__init__.py
--rw-r--r--   0 joel      (1000) joel      (1000)     2476 2023-04-18 08:55:35.000000 gitfluencer-0.1.3/gitfluencer/app.py
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-04-18 08:56:41.042553 gitfluencer-0.1.3/gitfluencer.egg-info/
--rw-r--r--   0 joel      (1000) joel      (1000)      755 2023-04-18 08:56:41.000000 gitfluencer-0.1.3/gitfluencer.egg-info/PKG-INFO
--rw-r--r--   0 joel      (1000) joel      (1000)      273 2023-04-18 08:56:41.000000 gitfluencer-0.1.3/gitfluencer.egg-info/SOURCES.txt
--rw-r--r--   0 joel      (1000) joel      (1000)        1 2023-04-18 08:56:41.000000 gitfluencer-0.1.3/gitfluencer.egg-info/dependency_links.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       53 2023-04-18 08:56:41.000000 gitfluencer-0.1.3/gitfluencer.egg-info/entry_points.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       23 2023-04-18 08:56:41.000000 gitfluencer-0.1.3/gitfluencer.egg-info/requires.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       12 2023-04-18 08:56:41.000000 gitfluencer-0.1.3/gitfluencer.egg-info/top_level.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       38 2023-04-18 08:56:41.042553 gitfluencer-0.1.3/setup.cfg
--rw-r--r--   0 joel      (1000) joel      (1000)     1065 2023-04-18 08:56:18.000000 gitfluencer-0.1.3/setup.py
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-04-18 09:33:48.507625 gitfluencer-0.1.4/
+-rw-r--r--   0 joel      (1000) joel      (1000)      755 2023-04-18 09:33:48.507625 gitfluencer-0.1.4/PKG-INFO
+-rw-r--r--   0 joel      (1000) joel      (1000)      951 2023-04-18 07:59:49.000000 gitfluencer-0.1.4/README.md
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-04-18 09:33:48.507625 gitfluencer-0.1.4/gitfluencer/
+-rw-r--r--   0 joel      (1000) joel      (1000)        0 2023-04-18 08:01:35.000000 gitfluencer-0.1.4/gitfluencer/__init__.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     2751 2023-04-18 09:33:16.000000 gitfluencer-0.1.4/gitfluencer/app.py
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-04-18 09:33:48.507625 gitfluencer-0.1.4/gitfluencer.egg-info/
+-rw-r--r--   0 joel      (1000) joel      (1000)      755 2023-04-18 09:33:48.000000 gitfluencer-0.1.4/gitfluencer.egg-info/PKG-INFO
+-rw-r--r--   0 joel      (1000) joel      (1000)      273 2023-04-18 09:33:48.000000 gitfluencer-0.1.4/gitfluencer.egg-info/SOURCES.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)        1 2023-04-18 09:33:48.000000 gitfluencer-0.1.4/gitfluencer.egg-info/dependency_links.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       53 2023-04-18 09:33:48.000000 gitfluencer-0.1.4/gitfluencer.egg-info/entry_points.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       23 2023-04-18 09:33:48.000000 gitfluencer-0.1.4/gitfluencer.egg-info/requires.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       12 2023-04-18 09:33:48.000000 gitfluencer-0.1.4/gitfluencer.egg-info/top_level.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       38 2023-04-18 09:33:48.508625 gitfluencer-0.1.4/setup.cfg
+-rw-r--r--   0 joel      (1000) joel      (1000)     1065 2023-04-18 09:33:32.000000 gitfluencer-0.1.4/setup.py
```

### Comparing `gitfluencer-0.1.3/PKG-INFO` & `gitfluencer-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitfluencer
-Version: 0.1.3
+Version: 0.1.4
 Summary: Utility tool for interacting with the GitHub platform
 Home-page: https://github.com/jjoeldaniel/gitfluencer
 Author: jjoeldaniel
 Author-email: joeldanielrico@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `gitfluencer-0.1.3/README.md` & `gitfluencer-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `gitfluencer-0.1.3/gitfluencer/app.py` & `gitfluencer-0.1.4/gitfluencer/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,47 +2,31 @@
 from rich import print
 from rich.console import Console
 from rich.table import Table
 from rich.prompt import Prompt, Confirm
 import os
 import requests
 
-# Get API token from environment variable or prompt for input
-api_token = os.getenv("API_TOKEN")
-if not api_token:
-    api_token = Prompt.ask(
-            "Please enter your GitHub API token: ",
-            password=True,
-            show_default=False,
-            show_choices=True)
-
-# Store API token as environment variable
-os.environ["API_TOKEN"] = api_token
-
-# Create API object from token
-git = Github(api_token)
-to_be_unfollowed = list()
 
-
-def unfollow_user(target_username: str):
+def unfollow_user(target_username: str, api_token: str):
     headers = {
         'Accept': 'application/vnd.github+json',
         'Authorization': f'Bearer {api_token}',
         'X-GitHub-Api-Version': '2022-11-28',
     }
 
     response = requests.delete(
         f'https://api.github.com/user/following/{target_username}',
         headers=headers
     )
 
     return response.status_code
 
 
-def print_list():
+def print_list(git: Github, to_be_unfollowed: list):
 
     # Table to be printed
     table = Table(title='List of non-followers')
     table.add_column('GitHub Username', style='green')
     table.add_column('Name (if available)', justify='right', style='cyan')
 
     # Build set of followers for the primary user
@@ -72,17 +56,40 @@
 
         y += 1
 
     console = Console()
     console.print(table)
 
 
-print_list()
+def main():
+
+    # Get API token from environment variable or prompt for input
+    api_token = os.getenv("GH_API_TOKEN")
+    if not api_token:
+        api_token = Prompt.ask(
+                "Please enter your GitHub API token: ",
+                password=True,
+                show_default=False,
+                show_choices=True)
+
+    # Store API token as environment variable
+    os.environ["GH_API_TOKEN"] = api_token
+
+    # Create API object from token
+    git = Github(api_token)
+    to_be_unfollowed = list()
+
+    print_list(git, to_be_unfollowed)
+
+    # Confirmation
+    prompt = Prompt.ask('Unfollow all? [y] [n]', choices=['y', 'n'])
+    if prompt == "y" or prompt == "yes":
+        confirm = Confirm.ask("Are you sure?")
+        if confirm:
+            for user in to_be_unfollowed:
+                unfollow_user(target_username=user, api_token=api_token)
+    elif prompt == "n" or prompt == "no":
+        print('Goodbye!')
+
 
-prompt = Prompt.ask('Unfollow all? [y] [n]', choices=['y', 'n'])
-if prompt == "y" or prompt == "yes":
-    confirm = Confirm.ask("Are you sure?")
-    if confirm:
-        for user in to_be_unfollowed:
-            unfollow_user(user)
-elif prompt == "n" or prompt == "no":
-    print('Goodbye!')
+if __name__ == "__main__":
+    main()
```

### Comparing `gitfluencer-0.1.3/gitfluencer.egg-info/PKG-INFO` & `gitfluencer-0.1.4/gitfluencer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitfluencer
-Version: 0.1.3
+Version: 0.1.4
 Summary: Utility tool for interacting with the GitHub platform
 Home-page: https://github.com/jjoeldaniel/gitfluencer
 Author: jjoeldaniel
 Author-email: joeldanielrico@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `gitfluencer-0.1.3/setup.py` & `gitfluencer-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gitfluencer',
-    version='0.1.3',
+    version='0.1.4',
     description='Utility tool for interacting with the GitHub platform',
     author='jjoeldaniel',
     author_email='joeldanielrico@gmail.com',
     url='https://github.com/jjoeldaniel/gitfluencer',
     packages=find_packages(),
     install_requires=[
         'PyGithub',
```

