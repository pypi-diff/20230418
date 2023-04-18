# Comparing `tmp/nlptoolssna-0.2.6.tar.gz` & `tmp/nlptoolssna-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.2.6.tar", last modified: Tue Apr 18 08:56:49 2023, max compression
+gzip compressed data, was "nlptoolssna-0.2.7.tar", last modified: Tue Apr 18 08:59:05 2023, max compression
```

## Comparing `nlptoolssna-0.2.6.tar` & `nlptoolssna-0.2.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 08:56:49.137338 nlptoolssna-0.2.6/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.2.6/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.2.6/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.2.6/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.2.6/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.2.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1821 2023-04-18 08:56:49.138651 nlptoolssna-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.2.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-18 08:56:49.088987 nlptoolssna-0.2.6/docs/
--rw-rw-rw-   0        0        0      629 2023-04-15 18:20:16.000000 nlptoolssna-0.2.6/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.2.6/docs/authors.rst
--rw-rw-rw-   0        0        0     4947 2023-04-15 18:20:16.000000 nlptoolssna-0.2.6/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-04-15 18:20:16.000000 nlptoolssna-0.2.6/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.2.6/docs/history.rst
--rw-rw-rw-   0        0        0      325 2023-04-15 18:20:16.000000 nlptoolssna-0.2.6/docs/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.2.6/docs/installation.rst
--rwxrwxrwx   0        0        0      806 2023-04-15 18:20:16.000000 nlptoolssna-0.2.6/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-04-15 18:20:16.000000 nlptoolssna-0.2.6/docs/readme.rst
--rw-rw-rw-   0        0        0       78 2023-04-15 18:20:16.000000 nlptoolssna-0.2.6/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-04-18 08:56:49.096740 nlptoolssna-0.2.6/nlptools/
-drwxrwxrwx   0        0        0        0 2023-04-18 08:56:49.099316 nlptoolssna-0.2.6/nlptools/DataDownload/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.2.6/nlptools/DataDownload/__init__.py
--rw-rw-rw-   0        0        0     1292 2023-04-18 08:51:18.000000 nlptoolssna-0.2.6/nlptools/DataDownload/downloader.py
--rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.2.6/nlptools/__init__.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.2.6/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:56:49.101349 nlptoolssna-0.2.6/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.2.6/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-04-18 08:56:49.115095 nlptoolssna-0.2.6/nlptools/morph/
--rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.2.6/nlptools/morph/__init__.py
--rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 nlptoolssna-0.2.6/nlptools/morph/charsets.py
--rw-rw-rw-   0        0        0     2489 2023-04-15 18:55:28.000000 nlptoolssna-0.2.6/nlptools/morph/lemmatizeSentence.py
--rw-rw-rw-   0        0        0     9372 2023-04-18 08:54:41.000000 nlptoolssna-0.2.6/nlptools/morph/morph_tagger.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.2.6/nlptools/morph/settings.py
--rw-rw-rw-   0        0        0      592 2023-04-15 18:51:58.000000 nlptoolssna-0.2.6/nlptools/morph/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.2.6/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:56:49.119127 nlptoolssna-0.2.6/nlptools/parse/
--rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.2.6/nlptools/parse/__init__.py
--rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.2.6/nlptools/parse/parser.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:56:49.132438 nlptoolssna-0.2.6/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1821 2023-04-18 08:56:48.000000 nlptoolssna-0.2.6/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      934 2023-04-18 08:56:48.000000 nlptoolssna-0.2.6/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 08:56:48.000000 nlptoolssna-0.2.6/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-18 08:56:48.000000 nlptoolssna-0.2.6/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.2.6/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       46 2023-04-18 08:56:48.000000 nlptoolssna-0.2.6/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-18 08:56:48.000000 nlptoolssna-0.2.6/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      403 2023-04-18 08:56:49.140471 nlptoolssna-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1614 2023-04-18 08:56:41.000000 nlptoolssna-0.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:56:49.137046 nlptoolssna-0.2.6/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.2.6/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.2.6/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:59:05.472862 nlptoolssna-0.2.7/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.2.7/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.2.7/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.2.7/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.2.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1821 2023-04-18 08:59:05.472862 nlptoolssna-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.2.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-18 08:59:05.429684 nlptoolssna-0.2.7/docs/
+-rw-rw-rw-   0        0        0      629 2023-04-15 18:20:16.000000 nlptoolssna-0.2.7/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.2.7/docs/authors.rst
+-rw-rw-rw-   0        0        0     4947 2023-04-15 18:20:16.000000 nlptoolssna-0.2.7/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-04-15 18:20:16.000000 nlptoolssna-0.2.7/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-04-15 18:20:16.000000 nlptoolssna-0.2.7/docs/history.rst
+-rw-rw-rw-   0        0        0      325 2023-04-15 18:20:16.000000 nlptoolssna-0.2.7/docs/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.2.7/docs/installation.rst
+-rwxrwxrwx   0        0        0      806 2023-04-15 18:20:16.000000 nlptoolssna-0.2.7/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-04-15 18:20:16.000000 nlptoolssna-0.2.7/docs/readme.rst
+-rw-rw-rw-   0        0        0       78 2023-04-15 18:20:16.000000 nlptoolssna-0.2.7/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-04-18 08:59:05.436656 nlptoolssna-0.2.7/nlptools/
+drwxrwxrwx   0        0        0        0 2023-04-18 08:59:05.438692 nlptoolssna-0.2.7/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.2.7/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     1292 2023-04-18 08:51:18.000000 nlptoolssna-0.2.7/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.2.7/nlptools/__init__.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.2.7/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:59:05.440691 nlptoolssna-0.2.7/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.2.7/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-04-18 08:59:05.451274 nlptoolssna-0.2.7/nlptools/morph/
+-rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.2.7/nlptools/morph/__init__.py
+-rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 nlptoolssna-0.2.7/nlptools/morph/charsets.py
+-rw-rw-rw-   0        0        0     2489 2023-04-15 18:55:28.000000 nlptoolssna-0.2.7/nlptools/morph/lemmatizeSentence.py
+-rw-rw-rw-   0        0        0     9372 2023-04-18 08:54:41.000000 nlptoolssna-0.2.7/nlptools/morph/morph_tagger.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.2.7/nlptools/morph/settings.py
+-rw-rw-rw-   0        0        0      592 2023-04-15 18:51:58.000000 nlptoolssna-0.2.7/nlptools/morph/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.2.7/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:59:05.453864 nlptoolssna-0.2.7/nlptools/parse/
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.2.7/nlptools/parse/__init__.py
+-rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.2.7/nlptools/parse/parser.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:59:05.467271 nlptoolssna-0.2.7/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1821 2023-04-18 08:59:05.000000 nlptoolssna-0.2.7/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2023-04-18 08:59:05.000000 nlptoolssna-0.2.7/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 08:59:05.000000 nlptoolssna-0.2.7/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-18 08:59:05.000000 nlptoolssna-0.2.7/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.2.7/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-04-18 08:59:05.000000 nlptoolssna-0.2.7/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-18 08:59:05.000000 nlptoolssna-0.2.7/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      403 2023-04-18 08:59:05.474875 nlptoolssna-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1601 2023-04-18 08:58:59.000000 nlptoolssna-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:59:05.471858 nlptoolssna-0.2.7/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.2.7/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.2.7/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.2.6/CONTRIBUTING.rst` & `nlptoolssna-0.2.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.6/LICENSE` & `nlptoolssna-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.6/PKG-INFO` & `nlptoolssna-0.2.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.2.6
+Version: 0.2.7
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.2.6/README.rst` & `nlptoolssna-0.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.6/docs/Makefile` & `nlptoolssna-0.2.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.6/docs/conf.py` & `nlptoolssna-0.2.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.6/docs/installation.rst` & `nlptoolssna-0.2.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.6/docs/make.bat` & `nlptoolssna-0.2.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.6/nlptools/DataDownload/downloader.py` & `nlptoolssna-0.2.7/nlptools/DataDownload/downloader.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.6/nlptools/data/my_data.pickle` & `nlptoolssna-0.2.7/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.6/nlptools/morph/charsets.py` & `nlptoolssna-0.2.7/nlptools/morph/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.6/nlptools/morph/lemmatizeSentence.py` & `nlptoolssna-0.2.7/nlptools/morph/lemmatizeSentence.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.6/nlptools/morph/morph_tagger.py` & `nlptoolssna-0.2.7/nlptools/morph/morph_tagger.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.6/nlptools/morph/tokenizers_words.py` & `nlptoolssna-0.2.7/nlptools/morph/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.6/nlptools/parse/parser.py` & `nlptoolssna-0.2.7/nlptools/parse/parser.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.6/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.2.7/nlptoolssna.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.2.6
+Version: 0.2.7
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.2.6/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.2.7/nlptoolssna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.2.6/setup.py` & `nlptoolssna-0.2.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 requirements = [
     'six',
     'farasapy',
     'tqdm',
     'requests',
     'regex',
-    'json',
     'pathlib'
 
 ]
 
 test_requirements = [ ]
 
 setup(
@@ -50,10 +49,10 @@
     include_package_data=True,
     keywords='nlptools',
     name='nlptoolssna',
     packages=find_packages(include=['nlptools', 'nlptools.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/eng-aomar/nlptools',
-    version='0.2.6',
+    version='0.2.7',
     zip_safe=False,
 )
```

