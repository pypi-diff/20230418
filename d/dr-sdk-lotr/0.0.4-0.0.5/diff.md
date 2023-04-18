# Comparing `tmp/dr-sdk-lotr-0.0.4.tar.gz` & `tmp/dr-sdk-lotr-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dr-sdk-lotr-0.0.4.tar", last modified: Mon Apr 17 20:54:44 2023, max compression
+gzip compressed data, was "dr-sdk-lotr-0.0.5.tar", last modified: Tue Apr 18 15:36:13 2023, max compression
```

## Comparing `dr-sdk-lotr-0.0.4.tar` & `dr-sdk-lotr-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-17 20:54:44.853938 dr-sdk-lotr-0.0.4/
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1072 2023-04-14 12:36:30.000000 dr-sdk-lotr-0.0.4/LICENCE.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)     3132 2023-04-17 20:54:44.853757 dr-sdk-lotr-0.0.4/PKG-INFO
--rw-r--r--   0 dannyreliford   (501) staff       (20)     2297 2023-04-14 13:34:32.000000 dr-sdk-lotr-0.0.4/README.md
-drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-17 20:54:44.850885 dr-sdk-lotr-0.0.4/dr_sdk_lotr/
--rw-r--r--   0 dannyreliford   (501) staff       (20)      110 2023-04-17 20:54:17.000000 dr-sdk-lotr-0.0.4/dr_sdk_lotr/__init__.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1573 2023-04-14 13:54:17.000000 dr-sdk-lotr-0.0.4/dr_sdk_lotr/books.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1588 2023-04-14 13:54:16.000000 dr-sdk-lotr-0.0.4/dr_sdk_lotr/chapters.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     2127 2023-04-14 12:45:06.000000 dr-sdk-lotr-0.0.4/dr_sdk_lotr/characters.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1646 2023-04-14 13:54:14.000000 dr-sdk-lotr-0.0.4/dr_sdk_lotr/movies.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1077 2023-04-14 12:45:44.000000 dr-sdk-lotr-0.0.4/dr_sdk_lotr/quotes.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)       40 2023-04-14 12:46:03.000000 dr-sdk-lotr-0.0.4/dr_sdk_lotr/settings.py
-drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-17 20:54:44.851734 dr-sdk-lotr-0.0.4/dr_sdk_lotr.egg-info/
--rw-r--r--   0 dannyreliford   (501) staff       (20)     3132 2023-04-17 20:54:44.000000 dr-sdk-lotr-0.0.4/dr_sdk_lotr.egg-info/PKG-INFO
--rw-r--r--   0 dannyreliford   (501) staff       (20)      522 2023-04-17 20:54:44.000000 dr-sdk-lotr-0.0.4/dr_sdk_lotr.egg-info/SOURCES.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)        1 2023-04-17 20:54:44.000000 dr-sdk-lotr-0.0.4/dr_sdk_lotr.egg-info/dependency_links.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)        9 2023-04-17 20:54:44.000000 dr-sdk-lotr-0.0.4/dr_sdk_lotr.egg-info/requires.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)       12 2023-04-17 20:54:44.000000 dr-sdk-lotr-0.0.4/dr_sdk_lotr.egg-info/top_level.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)       38 2023-04-17 20:54:44.853981 dr-sdk-lotr-0.0.4/setup.cfg
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1090 2023-04-17 20:54:30.000000 dr-sdk-lotr-0.0.4/setup.py
-drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-17 20:54:44.853352 dr-sdk-lotr-0.0.4/tests/
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1144 2023-04-14 13:36:41.000000 dr-sdk-lotr-0.0.4/tests/test_books.unittest.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1070 2023-04-14 13:36:50.000000 dr-sdk-lotr-0.0.4/tests/test_chapters.unittest.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1636 2023-04-14 13:36:57.000000 dr-sdk-lotr-0.0.4/tests/test_characters.unittest.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1086 2023-04-14 18:52:00.000000 dr-sdk-lotr-0.0.4/tests/test_movies_unittest.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)      925 2023-04-14 13:37:17.000000 dr-sdk-lotr-0.0.4/tests/test_quotes_unittest.py
+drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-18 15:36:13.429047 dr-sdk-lotr-0.0.5/
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1072 2023-04-14 12:36:30.000000 dr-sdk-lotr-0.0.5/LICENCE.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     3132 2023-04-18 15:36:13.428868 dr-sdk-lotr-0.0.5/PKG-INFO
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     2297 2023-04-14 13:34:32.000000 dr-sdk-lotr-0.0.5/README.md
+drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-18 15:36:13.424879 dr-sdk-lotr-0.0.5/dr_sdk_lotr/
+-rw-r--r--   0 dannyreliford   (501) staff       (20)        0 2023-04-17 21:15:00.000000 dr-sdk-lotr-0.0.5/dr_sdk_lotr/__init__.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1573 2023-04-14 13:54:17.000000 dr-sdk-lotr-0.0.5/dr_sdk_lotr/books.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1588 2023-04-14 13:54:16.000000 dr-sdk-lotr-0.0.5/dr_sdk_lotr/chapters.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     2127 2023-04-14 12:45:06.000000 dr-sdk-lotr-0.0.5/dr_sdk_lotr/characters.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1646 2023-04-14 13:54:14.000000 dr-sdk-lotr-0.0.5/dr_sdk_lotr/movies.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1077 2023-04-14 12:45:44.000000 dr-sdk-lotr-0.0.5/dr_sdk_lotr/quotes.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)       40 2023-04-14 12:46:03.000000 dr-sdk-lotr-0.0.5/dr_sdk_lotr/settings.py
+drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-18 15:36:13.425880 dr-sdk-lotr-0.0.5/dr_sdk_lotr.egg-info/
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     3132 2023-04-18 15:36:13.000000 dr-sdk-lotr-0.0.5/dr_sdk_lotr.egg-info/PKG-INFO
+-rw-r--r--   0 dannyreliford   (501) staff       (20)      522 2023-04-18 15:36:13.000000 dr-sdk-lotr-0.0.5/dr_sdk_lotr.egg-info/SOURCES.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)        1 2023-04-18 15:36:13.000000 dr-sdk-lotr-0.0.5/dr_sdk_lotr.egg-info/dependency_links.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)        9 2023-04-18 15:36:13.000000 dr-sdk-lotr-0.0.5/dr_sdk_lotr.egg-info/requires.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)       12 2023-04-18 15:36:13.000000 dr-sdk-lotr-0.0.5/dr_sdk_lotr.egg-info/top_level.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)       38 2023-04-18 15:36:13.429095 dr-sdk-lotr-0.0.5/setup.cfg
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1090 2023-04-18 15:35:33.000000 dr-sdk-lotr-0.0.5/setup.py
+drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-18 15:36:13.428260 dr-sdk-lotr-0.0.5/tests/
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1144 2023-04-14 13:36:41.000000 dr-sdk-lotr-0.0.5/tests/test_books.unittest.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1070 2023-04-14 13:36:50.000000 dr-sdk-lotr-0.0.5/tests/test_chapters.unittest.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1636 2023-04-14 13:36:57.000000 dr-sdk-lotr-0.0.5/tests/test_characters.unittest.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1086 2023-04-14 18:52:00.000000 dr-sdk-lotr-0.0.5/tests/test_movies_unittest.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)      925 2023-04-14 13:37:17.000000 dr-sdk-lotr-0.0.5/tests/test_quotes_unittest.py
```

### Comparing `dr-sdk-lotr-0.0.4/LICENCE.txt` & `dr-sdk-lotr-0.0.5/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `dr-sdk-lotr-0.0.4/PKG-INFO` & `dr-sdk-lotr-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dr-sdk-lotr
-Version: 0.0.4
+Version: 0.0.5
 Summary: SDK for interacting with the Lord of the Rings API
 Author: Daniel Reliford
 Author-email: dreliford@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dr-sdk-lotr-0.0.4/README.md` & `dr-sdk-lotr-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dr-sdk-lotr-0.0.4/dr_sdk_lotr/books.py` & `dr-sdk-lotr-0.0.5/dr_sdk_lotr/books.py`

 * *Files identical despite different names*

### Comparing `dr-sdk-lotr-0.0.4/dr_sdk_lotr/chapters.py` & `dr-sdk-lotr-0.0.5/dr_sdk_lotr/chapters.py`

 * *Files identical despite different names*

### Comparing `dr-sdk-lotr-0.0.4/dr_sdk_lotr/characters.py` & `dr-sdk-lotr-0.0.5/dr_sdk_lotr/characters.py`

 * *Files identical despite different names*

### Comparing `dr-sdk-lotr-0.0.4/dr_sdk_lotr/movies.py` & `dr-sdk-lotr-0.0.5/dr_sdk_lotr/movies.py`

 * *Files identical despite different names*

### Comparing `dr-sdk-lotr-0.0.4/dr_sdk_lotr/quotes.py` & `dr-sdk-lotr-0.0.5/dr_sdk_lotr/quotes.py`

 * *Files identical despite different names*

### Comparing `dr-sdk-lotr-0.0.4/dr_sdk_lotr.egg-info/PKG-INFO` & `dr-sdk-lotr-0.0.5/dr_sdk_lotr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dr-sdk-lotr
-Version: 0.0.4
+Version: 0.0.5
 Summary: SDK for interacting with the Lord of the Rings API
 Author: Daniel Reliford
 Author-email: dreliford@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dr-sdk-lotr-0.0.4/dr_sdk_lotr.egg-info/SOURCES.txt` & `dr-sdk-lotr-0.0.5/dr_sdk_lotr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dr-sdk-lotr-0.0.4/setup.py` & `dr-sdk-lotr-0.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='dr-sdk-lotr',
-    version='0.0.4',
+    version='0.0.5',
     description='SDK for interacting with the Lord of the Rings API',
     author='Daniel Reliford',
     author_email='dreliford@gmail.com',
     packages=setuptools.find_packages(),
     install_requires=['requests'],
     classifiers=[
         'Development Status :: 3 - Alpha',
```

### Comparing `dr-sdk-lotr-0.0.4/tests/test_books.unittest.py` & `dr-sdk-lotr-0.0.5/tests/test_books.unittest.py`

 * *Files identical despite different names*

### Comparing `dr-sdk-lotr-0.0.4/tests/test_chapters.unittest.py` & `dr-sdk-lotr-0.0.5/tests/test_chapters.unittest.py`

 * *Files identical despite different names*

### Comparing `dr-sdk-lotr-0.0.4/tests/test_characters.unittest.py` & `dr-sdk-lotr-0.0.5/tests/test_characters.unittest.py`

 * *Files identical despite different names*

### Comparing `dr-sdk-lotr-0.0.4/tests/test_movies_unittest.py` & `dr-sdk-lotr-0.0.5/tests/test_movies_unittest.py`

 * *Files identical despite different names*

### Comparing `dr-sdk-lotr-0.0.4/tests/test_quotes_unittest.py` & `dr-sdk-lotr-0.0.5/tests/test_quotes_unittest.py`

 * *Files identical despite different names*

