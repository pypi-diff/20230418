# Comparing `tmp/pandit-0.0.7.tar.gz` & `tmp/pandit-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandit-0.0.7.tar", last modified: Tue Feb 21 14:24:56 2023, max compression
+gzip compressed data, was "pandit-0.0.8.tar", last modified: Tue Apr 18 08:53:29 2023, max compression
```

## Comparing `pandit-0.0.7.tar` & `pandit-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:24:56.263181 pandit-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-21 14:24:50.000000 pandit-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-02-21 14:24:56.263181 pandit-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-02-21 14:24:50.000000 pandit-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:24:56.263181 pandit-0.0.7/pandit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-02-21 14:24:56.000000 pandit-0.0.7/pandit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-02-21 14:24:56.000000 pandit-0.0.7/pandit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 14:24:56.000000 pandit-0.0.7/pandit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 14:24:56.000000 pandit-0.0.7/pandit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-21 14:24:56.000000 pandit-0.0.7/pandit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-21 14:24:56.000000 pandit-0.0.7/pandit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-02-21 14:24:50.000000 pandit-0.0.7/pandit.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-21 14:24:56.263181 pandit-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-02-21 14:24:54.000000 pandit-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:53:29.517304 pandit-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-18 08:53:22.000000 pandit-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-18 08:53:29.517304 pandit-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-18 08:53:22.000000 pandit-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:53:29.517304 pandit-0.0.8/pandit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-18 08:53:29.000000 pandit-0.0.8/pandit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-18 08:53:29.000000 pandit-0.0.8/pandit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:53:29.000000 pandit-0.0.8/pandit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:53:29.000000 pandit-0.0.8/pandit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 08:53:29.000000 pandit-0.0.8/pandit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 08:53:29.000000 pandit-0.0.8/pandit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-04-18 08:53:22.000000 pandit-0.0.8/pandit.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-18 08:53:29.517304 pandit-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-18 08:53:27.000000 pandit-0.0.8/setup.py
```

### Comparing `pandit-0.0.7/LICENSE` & `pandit-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pandit-0.0.7/PKG-INFO` & `pandit-0.0.8/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,48 @@
-Metadata-Version: 2.1
-Name: pandit
-Version: 0.0.7
-Summary: Pandas with some cool additional features
-Home-page: https://github.com/sileod/pandit
-Author: sileod
-License: GPL
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pandit ☸️ 
+# pandit ☸️ pandas utils 
 Pandas with some cool additional features
 
 ### Installation and usage
 `pip install pandit`
 ```python
 import pandas as pd, import pandit
 # or 
 import pandit as pd
 
 df=pd.read_tsv(path)
 df.sieve(x=3).show()
+#Pandas behaves normally otherwise
 ```
 
 ### `sieve`
 ```python
-df.sieve(column=value) # returns df rows where column equals value
-df.sieve(column=[value1,value2]) # returns df rows where column is value1 or value2
+df.sieve(column1=value1, columns2=value2)
+# returns df rows where column equals value - if value is not a list, otherwise:
+df.sieve(column3=[value1,value2])
+# returns df rows where column is value1 or value2; use [[value1,value2]] to match lists
 # It's like pd.query but with a pythonic syntax instead of the sql string.
 ```
 
 ### `show`
 ```python
-df.show() # shows multiple rows column by column (one line per column) with nice formatting
-df.rshow(n) # random sample of size n
+df.show() # shows multiple rows column by column (one line per column) with nice formatting, one line per column
+# ideal for inspecting NLP datasets
+df.rshow(n) # random sample of size n (default is 20)
 ```
 
 Also:
 
+### `bold_max`
+bold max float values `df.bold_max().to_latex()`
 ### `read_tsv`
 `read_csv` with `sep='\t'` for lazy persons
 ### `read_jsonl`
+### `read`
+`read_{extension}` where extension is extracted from the input path (.csv = read_csv)
 ### `read_wandb(project_name)`
-### `drop_constant`
+### `drop_constant_column`
 drop columns that are constant
+### `to_dropbox(df, path, format=None, token=None,**kwargs)`
+Save dataframe to dropbox
+### FAQ
+- Should I use pandit in production ?
+No.
```

### Comparing `pandit-0.0.7/pandit.egg-info/PKG-INFO` & `pandit-0.0.8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,58 @@
 Metadata-Version: 2.1
 Name: pandit
-Version: 0.0.7
+Version: 0.0.8
 Summary: Pandas with some cool additional features
 Home-page: https://github.com/sileod/pandit
 Author: sileod
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# pandit ☸️ 
+# pandit ☸️ pandas utils 
 Pandas with some cool additional features
 
 ### Installation and usage
 `pip install pandit`
 ```python
 import pandas as pd, import pandit
 # or 
 import pandit as pd
 
 df=pd.read_tsv(path)
 df.sieve(x=3).show()
+#Pandas behaves normally otherwise
 ```
 
 ### `sieve`
 ```python
-df.sieve(column=value) # returns df rows where column equals value
-df.sieve(column=[value1,value2]) # returns df rows where column is value1 or value2
+df.sieve(column1=value1, columns2=value2)
+# returns df rows where column equals value - if value is not a list, otherwise:
+df.sieve(column3=[value1,value2])
+# returns df rows where column is value1 or value2; use [[value1,value2]] to match lists
 # It's like pd.query but with a pythonic syntax instead of the sql string.
 ```
 
 ### `show`
 ```python
-df.show() # shows multiple rows column by column (one line per column) with nice formatting
-df.rshow(n) # random sample of size n
+df.show() # shows multiple rows column by column (one line per column) with nice formatting, one line per column
+# ideal for inspecting NLP datasets
+df.rshow(n) # random sample of size n (default is 20)
 ```
 
 Also:
 
+### `bold_max`
+bold max float values `df.bold_max().to_latex()`
 ### `read_tsv`
 `read_csv` with `sep='\t'` for lazy persons
 ### `read_jsonl`
+### `read`
+`read_{extension}` where extension is extracted from the input path (.csv = read_csv)
 ### `read_wandb(project_name)`
-### `drop_constant`
+### `drop_constant_column`
 drop columns that are constant
+### `to_dropbox(df, path, format=None, token=None,**kwargs)`
+Save dataframe to dropbox
+### FAQ
+- Should I use pandit in production ?
+No.
```

### Comparing `pandit-0.0.7/setup.py` & `pandit-0.0.8/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='pandit',
-      version='v0.0.7',
+      version='v0.0.8',
       description='Pandas with some cool additional features',
       url='https://github.com/sileod/pandit',
       author='sileod',
       license='GPL',
       install_requires=['pandas'],
       py_modules=['pandit'],
       long_description=long_description,
```

