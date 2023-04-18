# Comparing `tmp/tinote-1.1.1.tar.gz` & `tmp/tinote-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinote-1.1.1.tar", last modified: Tue Apr 18 20:23:03 2023, max compression
+gzip compressed data, was "tinote-1.1.2.tar", last modified: Tue Apr 18 21:54:28 2023, max compression
```

## Comparing `tinote-1.1.1.tar` & `tinote-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:23:03.233463 tinote-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-18 20:23:03.233463 tinote-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-18 20:22:51.000000 tinote-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:23:03.233463 tinote-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-18 20:22:51.000000 tinote-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:23:03.233463 tinote-1.1.1/tinote/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:22:51.000000 tinote-1.1.1/tinote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-04-18 20:22:51.000000 tinote-1.1.1/tinote/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-18 20:22:51.000000 tinote-1.1.1/tinote/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:23:03.233463 tinote-1.1.1/tinote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-18 20:23:03.000000 tinote-1.1.1/tinote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-18 20:23:03.000000 tinote-1.1.1/tinote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:23:03.000000 tinote-1.1.1/tinote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 20:23:03.000000 tinote-1.1.1/tinote.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 20:23:03.000000 tinote-1.1.1/tinote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:54:28.104280 tinote-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-18 21:54:28.104280 tinote-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-18 21:54:16.000000 tinote-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 21:54:28.104280 tinote-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-18 21:54:16.000000 tinote-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:54:28.104280 tinote-1.1.2/tinote/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:54:16.000000 tinote-1.1.2/tinote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-04-18 21:54:16.000000 tinote-1.1.2/tinote/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-18 21:54:16.000000 tinote-1.1.2/tinote/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:54:28.104280 tinote-1.1.2/tinote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-18 21:54:28.000000 tinote-1.1.2/tinote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-18 21:54:28.000000 tinote-1.1.2/tinote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:54:28.000000 tinote-1.1.2/tinote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 21:54:28.000000 tinote-1.1.2/tinote.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 21:54:28.000000 tinote-1.1.2/tinote.egg-info/top_level.txt
```

### Comparing `tinote-1.1.1/PKG-INFO` & `tinote-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinote
-Version: 1.1.1
+Version: 1.1.2
 Summary: A command-line note-taking tool
 Home-page: https://github.com/aPeter1/tinote
 Author: Alec Petersen
 Author-email: k.alecpetersen@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,17 +15,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Terminals
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-![Logo](assets/color-logo-no-background.png)
+![Logo](https://raw.githubusercontent.com/aPeter1/tinote/main/assets/color-logo-no-background.png)
 
-Tinote is a lightweight command-line note-taking tool, designed for quick and easy note management. Keep track of your thoughts, ideas, or reminders directly from the terminal.
+Tinote is light-weight command-line note-taking tool, designed for quick and easy note management. Keep track of your thoughts, ideas, or reminders directly from the terminal.
 
 ## Installation
 
 Install Tinote using pip:
 
 ```bash
 pip install tinote
```

### Comparing `tinote-1.1.1/README.md` & `tinote-1.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-![Logo](assets/color-logo-no-background.png)
+![Logo](https://raw.githubusercontent.com/aPeter1/tinote/main/assets/color-logo-no-background.png)
 
-Tinote is a lightweight command-line note-taking tool, designed for quick and easy note management. Keep track of your thoughts, ideas, or reminders directly from the terminal.
+Tinote is light-weight command-line note-taking tool, designed for quick and easy note management. Keep track of your thoughts, ideas, or reminders directly from the terminal.
 
 ## Installation
 
 Install Tinote using pip:
 
 ```bash
 pip install tinote
```

### Comparing `tinote-1.1.1/setup.py` & `tinote-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `tinote-1.1.1/tinote/main.py` & `tinote-1.1.2/tinote/main.py`

 * *Files identical despite different names*

### Comparing `tinote-1.1.1/tinote/update.py` & `tinote-1.1.2/tinote/update.py`

 * *Files identical despite different names*

### Comparing `tinote-1.1.1/tinote.egg-info/PKG-INFO` & `tinote-1.1.2/tinote.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinote
-Version: 1.1.1
+Version: 1.1.2
 Summary: A command-line note-taking tool
 Home-page: https://github.com/aPeter1/tinote
 Author: Alec Petersen
 Author-email: k.alecpetersen@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,17 +15,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Terminals
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-![Logo](assets/color-logo-no-background.png)
+![Logo](https://raw.githubusercontent.com/aPeter1/tinote/main/assets/color-logo-no-background.png)
 
-Tinote is a lightweight command-line note-taking tool, designed for quick and easy note management. Keep track of your thoughts, ideas, or reminders directly from the terminal.
+Tinote is light-weight command-line note-taking tool, designed for quick and easy note management. Keep track of your thoughts, ideas, or reminders directly from the terminal.
 
 ## Installation
 
 Install Tinote using pip:
 
 ```bash
 pip install tinote
```

