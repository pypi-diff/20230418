# Comparing `tmp/arxiv-1.4.5.tar.gz` & `tmp/arxiv-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arxiv-1.4.5.tar", last modified: Mon Apr 17 00:45:59 2023, max compression
+gzip compressed data, was "arxiv-1.4.6.tar", last modified: Tue Apr 18 21:46:57 2023, max compression
```

## Comparing `arxiv-1.4.5.tar` & `arxiv-1.4.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-17 00:45:59.443871 arxiv-1.4.5/
--rw-r--r--   0 lukas      (501) staff       (20)     1056 2018-08-22 17:46:13.000000 arxiv-1.4.5/LICENSE.txt
--rw-r--r--   0 lukas      (501) staff       (20)     7865 2023-04-17 00:45:59.444040 arxiv-1.4.5/PKG-INFO
--rw-r--r--   0 lukas      (501) staff       (20)     7363 2023-03-12 19:09:15.000000 arxiv-1.4.5/README.md
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-17 00:45:59.436610 arxiv-1.4.5/arxiv/
--rw-r--r--   0 lukas      (501) staff       (20)       35 2022-01-26 03:22:05.000000 arxiv-1.4.5/arxiv/__init__.py
--rw-r--r--   0 lukas      (501) staff       (20)    26587 2023-04-17 00:44:38.000000 arxiv-1.4.5/arxiv/arxiv.py
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-17 00:45:59.440383 arxiv-1.4.5/arxiv.egg-info/
--rw-r--r--   0 lukas      (501) staff       (20)     7865 2023-04-17 00:45:59.000000 arxiv-1.4.5/arxiv.egg-info/PKG-INFO
--rw-r--r--   0 lukas      (501) staff       (20)      305 2023-04-17 00:45:59.000000 arxiv-1.4.5/arxiv.egg-info/SOURCES.txt
--rw-r--r--   0 lukas      (501) staff       (20)        1 2023-04-17 00:45:59.000000 arxiv-1.4.5/arxiv.egg-info/dependency_links.txt
--rw-r--r--   0 lukas      (501) staff       (20)       11 2023-04-17 00:45:59.000000 arxiv-1.4.5/arxiv.egg-info/requires.txt
--rw-r--r--   0 lukas      (501) staff       (20)        6 2023-04-17 00:45:59.000000 arxiv-1.4.5/arxiv.egg-info/top_level.txt
--rw-r--r--   0 lukas      (501) staff       (20)      146 2023-04-17 00:45:59.444724 arxiv-1.4.5/setup.cfg
--rw-r--r--   0 lukas      (501) staff       (20)      890 2023-04-17 00:44:38.000000 arxiv-1.4.5/setup.py
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-17 00:45:59.443189 arxiv-1.4.5/tests/
--rw-r--r--   0 lukas      (501) staff       (20)     1008 2021-08-18 02:16:12.000000 arxiv-1.4.5/tests/test_api_bugs.py
--rw-r--r--   0 lukas      (501) staff       (20)     7417 2023-02-01 03:02:02.000000 arxiv-1.4.5/tests/test_client.py
--rw-r--r--   0 lukas      (501) staff       (20)     1213 2022-01-26 03:22:05.000000 arxiv-1.4.5/tests/test_download.py
--rw-r--r--   0 lukas      (501) staff       (20)     4098 2021-08-18 02:16:12.000000 arxiv-1.4.5/tests/test_result.py
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-18 21:46:57.986996 arxiv-1.4.6/
+-rw-r--r--   0 lukas      (501) staff       (20)     1056 2018-08-22 17:46:13.000000 arxiv-1.4.6/LICENSE.txt
+-rw-r--r--   0 lukas      (501) staff       (20)     7839 2023-04-18 21:46:57.987171 arxiv-1.4.6/PKG-INFO
+-rw-r--r--   0 lukas      (501) staff       (20)     7314 2023-04-18 21:41:18.000000 arxiv-1.4.6/README.md
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-18 21:46:57.979994 arxiv-1.4.6/arxiv/
+-rw-r--r--   0 lukas      (501) staff       (20)       35 2023-04-18 21:25:11.000000 arxiv-1.4.6/arxiv/__init__.py
+-rw-r--r--   0 lukas      (501) staff       (20)    26587 2023-04-17 00:44:38.000000 arxiv-1.4.6/arxiv/arxiv.py
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-18 21:46:57.983257 arxiv-1.4.6/arxiv.egg-info/
+-rw-r--r--   0 lukas      (501) staff       (20)     7839 2023-04-18 21:46:57.000000 arxiv-1.4.6/arxiv.egg-info/PKG-INFO
+-rw-r--r--   0 lukas      (501) staff       (20)      305 2023-04-18 21:46:57.000000 arxiv-1.4.6/arxiv.egg-info/SOURCES.txt
+-rw-r--r--   0 lukas      (501) staff       (20)        1 2023-04-18 21:46:57.000000 arxiv-1.4.6/arxiv.egg-info/dependency_links.txt
+-rw-r--r--   0 lukas      (501) staff       (20)       11 2023-04-18 21:46:57.000000 arxiv-1.4.6/arxiv.egg-info/requires.txt
+-rw-r--r--   0 lukas      (501) staff       (20)        6 2023-04-18 21:46:57.000000 arxiv-1.4.6/arxiv.egg-info/top_level.txt
+-rw-r--r--   0 lukas      (501) staff       (20)      114 2023-04-18 21:46:57.987767 arxiv-1.4.6/setup.cfg
+-rw-r--r--   0 lukas      (501) staff       (20)      917 2023-04-18 21:41:18.000000 arxiv-1.4.6/setup.py
+drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-04-18 21:46:57.986400 arxiv-1.4.6/tests/
+-rw-r--r--   0 lukas      (501) staff       (20)     1008 2021-08-18 02:16:12.000000 arxiv-1.4.6/tests/test_api_bugs.py
+-rw-r--r--   0 lukas      (501) staff       (20)     7417 2023-02-01 03:02:02.000000 arxiv-1.4.6/tests/test_client.py
+-rw-r--r--   0 lukas      (501) staff       (20)     1213 2022-01-26 03:22:05.000000 arxiv-1.4.6/tests/test_download.py
+-rw-r--r--   0 lukas      (501) staff       (20)     4098 2023-04-18 20:55:02.000000 arxiv-1.4.6/tests/test_result.py
```

### Comparing `arxiv-1.4.5/LICENSE.txt` & `arxiv-1.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arxiv-1.4.5/PKG-INFO` & `arxiv-1.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: arxiv
-Version: 1.4.5
+Version: 1.4.6
 Summary: Python wrapper for the arXiv API: http://arxiv.org/help/api/
 Home-page: https://github.com/lukasschwab/arxiv.py
 Author: Lukas Schwab
 Author-email: lukas.schwab@gmail.com
 License: MIT
 Keywords: arxiv api wrapper academic journals papers
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# arxiv.py [![Python 3.6](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/) [![PyPI](https://img.shields.io/pypi/v/arxiv)](https://pypi.org/project/arxiv/) [![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/lukasschwab/arxiv.py/python-package.yml?branch=master)](https://github.com/lukasschwab/arxiv.py/actions?query=branch%3Amaster)
+# arxiv.py [![PyPI](https://img.shields.io/pypi/v/arxiv)](https://pypi.org/project/arxiv/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/arxiv) [![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/lukasschwab/arxiv.py/python-package.yml?branch=master)](https://github.com/lukasschwab/arxiv.py/actions?query=branch%3Amaster)
 
 Python wrapper for [the arXiv API](http://arxiv.org/help/api/index).
 
 ## Quick links
 
 + [Full package documentation](http://lukasschwab.me/arxiv.py/index.html)
 + [Example: fetching results](#example-fetching-results): the most common usage.
```

### Comparing `arxiv-1.4.5/README.md` & `arxiv-1.4.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# arxiv.py [![Python 3.6](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/) [![PyPI](https://img.shields.io/pypi/v/arxiv)](https://pypi.org/project/arxiv/) [![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/lukasschwab/arxiv.py/python-package.yml?branch=master)](https://github.com/lukasschwab/arxiv.py/actions?query=branch%3Amaster)
+# arxiv.py [![PyPI](https://img.shields.io/pypi/v/arxiv)](https://pypi.org/project/arxiv/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/arxiv) [![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/lukasschwab/arxiv.py/python-package.yml?branch=master)](https://github.com/lukasschwab/arxiv.py/actions?query=branch%3Amaster)
 
 Python wrapper for [the arXiv API](http://arxiv.org/help/api/index).
 
 ## Quick links
 
 + [Full package documentation](http://lukasschwab.me/arxiv.py/index.html)
 + [Example: fetching results](#example-fetching-results): the most common usage.
```

### Comparing `arxiv-1.4.5/arxiv/arxiv.py` & `arxiv-1.4.6/arxiv/arxiv.py`

 * *Files identical despite different names*

### Comparing `arxiv-1.4.5/arxiv.egg-info/PKG-INFO` & `arxiv-1.4.6/arxiv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: arxiv
-Version: 1.4.5
+Version: 1.4.6
 Summary: Python wrapper for the arXiv API: http://arxiv.org/help/api/
 Home-page: https://github.com/lukasschwab/arxiv.py
 Author: Lukas Schwab
 Author-email: lukas.schwab@gmail.com
 License: MIT
 Keywords: arxiv api wrapper academic journals papers
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# arxiv.py [![Python 3.6](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/) [![PyPI](https://img.shields.io/pypi/v/arxiv)](https://pypi.org/project/arxiv/) [![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/lukasschwab/arxiv.py/python-package.yml?branch=master)](https://github.com/lukasschwab/arxiv.py/actions?query=branch%3Amaster)
+# arxiv.py [![PyPI](https://img.shields.io/pypi/v/arxiv)](https://pypi.org/project/arxiv/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/arxiv) [![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/lukasschwab/arxiv.py/python-package.yml?branch=master)](https://github.com/lukasschwab/arxiv.py/actions?query=branch%3Amaster)
 
 Python wrapper for [the arXiv API](http://arxiv.org/help/api/index).
 
 ## Quick links
 
 + [Full package documentation](http://lukasschwab.me/arxiv.py/index.html)
 + [Example: fetching results](#example-fetching-results): the most common usage.
```

### Comparing `arxiv-1.4.5/setup.py` & `arxiv-1.4.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup
 
-version = '1.4.5'
+version = '1.4.6'
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='arxiv',
     version=version,
     packages=['arxiv'],
     # dependencies
+    python_requires='>=3.7',
     install_requires=['feedparser'],
     tests_require=[
         'pytest',
         'pdoc',
-        'flake8'
+        'ruff'
     ],
     # metadata for upload to PyPI
     author='Lukas Schwab',
     author_email='lukas.schwab@gmail.com',
     description='Python wrapper for the arXiv API: http://arxiv.org/help/api/',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `arxiv-1.4.5/tests/test_api_bugs.py` & `arxiv-1.4.6/tests/test_api_bugs.py`

 * *Files identical despite different names*

### Comparing `arxiv-1.4.5/tests/test_client.py` & `arxiv-1.4.6/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `arxiv-1.4.5/tests/test_download.py` & `arxiv-1.4.6/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `arxiv-1.4.5/tests/test_result.py` & `arxiv-1.4.6/tests/test_result.py`

 * *Files identical despite different names*

