# Comparing `tmp/nlptoolssna-0.2.3.tar.gz` & `tmp/nlptoolssna-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.2.3.tar", last modified: Tue Apr 18 08:39:04 2023, max compression
+gzip compressed data, was "nlptoolssna-0.2.4.tar", last modified: Tue Apr 18 08:51:28 2023, max compression
```

## Comparing `nlptoolssna-0.2.3.tar` & `nlptoolssna-0.2.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 08:39:04.157757 nlptoolssna-0.2.3/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1821 2023-04-18 08:39:04.157757 nlptoolssna-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-18 08:39:04.101660 nlptoolssna-0.2.3/docs/
--rw-rw-rw-   0        0        0      629 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/docs/authors.rst
--rw-rw-rw-   0        0        0     4947 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/docs/history.rst
--rw-rw-rw-   0        0        0      325 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/docs/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/docs/installation.rst
--rwxrwxrwx   0        0        0      806 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/docs/readme.rst
--rw-rw-rw-   0        0        0       78 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-04-18 08:39:04.108326 nlptoolssna-0.2.3/nlptools/
-drwxrwxrwx   0        0        0        0 2023-04-18 08:39:04.110327 nlptoolssna-0.2.3/nlptools/DataDownload/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.2.3/nlptools/DataDownload/__init__.py
--rw-rw-rw-   0        0        0     1304 2023-04-18 08:31:42.000000 nlptoolssna-0.2.3/nlptools/DataDownload/downloader.py
--rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/nlptools/__init__.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:39:04.118681 nlptoolssna-0.2.3/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.2.3/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-04-18 08:39:04.131176 nlptoolssna-0.2.3/nlptools/morph/
--rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.2.3/nlptools/morph/__init__.py
--rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 nlptoolssna-0.2.3/nlptools/morph/charsets.py
--rw-rw-rw-   0        0        0     2489 2023-04-15 18:55:28.000000 nlptoolssna-0.2.3/nlptools/morph/lemmatizeSentence.py
--rw-rw-rw-   0        0        0     9426 2023-04-18 08:38:01.000000 nlptoolssna-0.2.3/nlptools/morph/morph_tagger.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.2.3/nlptools/morph/settings.py
--rw-rw-rw-   0        0        0      592 2023-04-15 18:51:58.000000 nlptoolssna-0.2.3/nlptools/morph/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:39:04.136423 nlptoolssna-0.2.3/nlptools/parse/
--rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.2.3/nlptools/parse/__init__.py
--rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.2.3/nlptools/parse/parser.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:39:04.151816 nlptoolssna-0.2.3/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1821 2023-04-18 08:39:03.000000 nlptoolssna-0.2.3/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      934 2023-04-18 08:39:03.000000 nlptoolssna-0.2.3/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 08:39:03.000000 nlptoolssna-0.2.3/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-18 08:39:03.000000 nlptoolssna-0.2.3/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.2.3/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       45 2023-04-18 08:39:03.000000 nlptoolssna-0.2.3/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-18 08:39:03.000000 nlptoolssna-0.2.3/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      403 2023-04-18 08:39:04.159738 nlptoolssna-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1611 2023-04-18 08:38:23.000000 nlptoolssna-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:39:04.155762 nlptoolssna-0.2.3/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.2.3/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:51:28.379469 nlptoolssna-0.2.4/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.2.4/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.2.4/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.2.4/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1821 2023-04-18 08:51:28.379469 nlptoolssna-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.2.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-18 08:51:28.327692 nlptoolssna-0.2.4/docs/
+-rw-rw-rw-   0        0        0      629 2023-04-15 18:20:16.000000 nlptoolssna-0.2.4/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.2.4/docs/authors.rst
+-rw-rw-rw-   0        0        0     4947 2023-04-15 18:20:16.000000 nlptoolssna-0.2.4/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-04-15 18:20:16.000000 nlptoolssna-0.2.4/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.2.4/docs/history.rst
+-rw-rw-rw-   0        0        0      325 2023-04-15 18:20:16.000000 nlptoolssna-0.2.4/docs/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.2.4/docs/installation.rst
+-rwxrwxrwx   0        0        0      806 2023-04-15 18:20:16.000000 nlptoolssna-0.2.4/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-04-15 18:20:16.000000 nlptoolssna-0.2.4/docs/readme.rst
+-rw-rw-rw-   0        0        0       78 2023-04-15 18:20:16.000000 nlptoolssna-0.2.4/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-04-18 08:51:28.333247 nlptoolssna-0.2.4/nlptools/
+drwxrwxrwx   0        0        0        0 2023-04-18 08:51:28.337245 nlptoolssna-0.2.4/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.2.4/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     1292 2023-04-18 08:51:18.000000 nlptoolssna-0.2.4/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.2.4/nlptools/__init__.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.2.4/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:51:28.339321 nlptoolssna-0.2.4/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.2.4/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-04-18 08:51:28.351628 nlptoolssna-0.2.4/nlptools/morph/
+-rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.2.4/nlptools/morph/__init__.py
+-rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 nlptoolssna-0.2.4/nlptools/morph/charsets.py
+-rw-rw-rw-   0        0        0     2489 2023-04-15 18:55:28.000000 nlptoolssna-0.2.4/nlptools/morph/lemmatizeSentence.py
+-rw-rw-rw-   0        0        0     9426 2023-04-18 08:38:01.000000 nlptoolssna-0.2.4/nlptools/morph/morph_tagger.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.2.4/nlptools/morph/settings.py
+-rw-rw-rw-   0        0        0      592 2023-04-15 18:51:58.000000 nlptoolssna-0.2.4/nlptools/morph/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.2.4/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:51:28.355921 nlptoolssna-0.2.4/nlptools/parse/
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.2.4/nlptools/parse/__init__.py
+-rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.2.4/nlptools/parse/parser.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:51:28.372310 nlptoolssna-0.2.4/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1821 2023-04-18 08:51:28.000000 nlptoolssna-0.2.4/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2023-04-18 08:51:28.000000 nlptoolssna-0.2.4/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 08:51:28.000000 nlptoolssna-0.2.4/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-18 08:51:28.000000 nlptoolssna-0.2.4/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.2.4/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       61 2023-04-18 08:51:28.000000 nlptoolssna-0.2.4/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-18 08:51:28.000000 nlptoolssna-0.2.4/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      403 2023-04-18 08:51:28.381469 nlptoolssna-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1643 2023-04-18 08:51:13.000000 nlptoolssna-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:51:28.376869 nlptoolssna-0.2.4/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.2.4/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.2.4/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.2.3/CONTRIBUTING.rst` & `nlptoolssna-0.2.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.3/LICENSE` & `nlptoolssna-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.3/PKG-INFO` & `nlptoolssna-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.2.3/README.rst` & `nlptoolssna-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.3/docs/Makefile` & `nlptoolssna-0.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.3/docs/conf.py` & `nlptoolssna-0.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.3/docs/installation.rst` & `nlptoolssna-0.2.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.3/docs/make.bat` & `nlptoolssna-0.2.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.3/nlptools/DataDownload/downloader.py` & `nlptoolssna-0.2.4/nlptools/DataDownload/downloader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 import os
 import sys
 from pathlib import Path
 import requests  
 import zipfile
 
 downloadLink = 'https://github.com/eng-aomar/ts/raw/main/my_data.pickle'
```

### Comparing `nlptoolssna-0.2.3/nlptools/data/my_data.pickle` & `nlptoolssna-0.2.4/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.3/nlptools/morph/charsets.py` & `nlptoolssna-0.2.4/nlptools/morph/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.3/nlptools/morph/lemmatizeSentence.py` & `nlptoolssna-0.2.4/nlptools/morph/lemmatizeSentence.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.3/nlptools/morph/morph_tagger.py` & `nlptoolssna-0.2.4/nlptools/morph/morph_tagger.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.3/nlptools/morph/tokenizers_words.py` & `nlptoolssna-0.2.4/nlptools/morph/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.3/nlptools/parse/parser.py` & `nlptoolssna-0.2.4/nlptools/parse/parser.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.3/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.2.4/nlptoolssna.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.2.3/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.2.4/nlptoolssna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.3/setup.py` & `nlptoolssna-0.2.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 requirements = [
     'six',
     'farasapy',
     'tqdm',
     'requests',
     'regex',
     'json',
-    'urllib'
+    'urllib',
+    'pathlib',
+    'zipfile'
 ]
 
 test_requirements = [ ]
 
 setup(
     author="Alaa' Omar",
     author_email='alaa.omer2009@gmail.com',
@@ -49,10 +51,10 @@
     include_package_data=True,
     keywords='nlptools',
     name='nlptoolssna',
     packages=find_packages(include=['nlptools', 'nlptools.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/eng-aomar/nlptools',
-    version='0.2.3',
+    version='0.2.4',
     zip_safe=False,
 )
```

