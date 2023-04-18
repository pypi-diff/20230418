# Comparing `tmp/Internationalize-0.0.1a1-py2.py3-none-any.whl.zip` & `tmp/Internationalize-0.0.2a2.win-amd64.zip`

## zipinfo {}

```diff
@@ -1,7 +1,18 @@
-Zip file size: 1819 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat       23 b- defN 23-Apr-18 17:18 internationalize/__init__.py
--rw-rw-rw-  2.0 fat     1737 b- defN 23-Apr-18 17:20 Internationalize-0.0.1a1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-18 17:20 Internationalize-0.0.1a1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Apr-18 17:20 Internationalize-0.0.1a1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      426 b- defN 23-Apr-18 17:20 Internationalize-0.0.1a1.dist-info/RECORD
-5 files, 2313 bytes uncompressed, 1017 bytes compressed:  56.0%
+Zip file size: 6629 bytes, number of entries: 16
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-18 20:27 Python39/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-18 20:27 Python39/Lib/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-18 20:27 Python39/Lib/site-packages/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-18 20:27 Python39/Lib/site-packages/internationalize/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-18 20:27 Python39/Lib/site-packages/Internationalize-0.0.2a2-py3.9.egg-info/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-18 20:27 Python39/Lib/site-packages/internationalize/__pycache__/
+-rw-rw-rw-  2.0 fat     1238 b- defN 23-Apr-18 20:26 Python39/Lib/site-packages/internationalize/configure.py
+-rw-rw-rw-  2.0 fat      692 b- defN 23-Apr-18 20:23 Python39/Lib/site-packages/internationalize/provider.py
+-rw-rw-rw-  2.0 fat      149 b- defN 23-Apr-18 20:23 Python39/Lib/site-packages/internationalize/__init__.py
+-rw-rw-rw-  2.0 fat     1292 b- defN 23-Apr-18 20:27 Python39/Lib/site-packages/internationalize/__pycache__/configure.cpython-39.pyc
+-rw-rw-rw-  2.0 fat      946 b- defN 23-Apr-18 20:27 Python39/Lib/site-packages/internationalize/__pycache__/provider.cpython-39.pyc
+-rw-rw-rw-  2.0 fat      327 b- defN 23-Apr-18 20:27 Python39/Lib/site-packages/internationalize/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Apr-18 20:27 Python39/Lib/site-packages/Internationalize-0.0.2a2-py3.9.egg-info/dependency_links.txt
+-rw-rw-rw-  2.0 fat     3107 b- defN 23-Apr-18 20:27 Python39/Lib/site-packages/Internationalize-0.0.2a2-py3.9.egg-info/PKG-INFO
+-rw-rw-rw-  2.0 fat      276 b- defN 23-Apr-18 20:27 Python39/Lib/site-packages/Internationalize-0.0.2a2-py3.9.egg-info/SOURCES.txt
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Apr-18 20:27 Python39/Lib/site-packages/Internationalize-0.0.2a2-py3.9.egg-info/top_level.txt
+16 files, 8045 bytes uncompressed, 3511 bytes compressed:  56.4%
```

## zipnote {}

```diff
@@ -1,16 +1,49 @@
-Filename: internationalize/__init__.py
+Filename: Python39/
 Comment: 
 
-Filename: Internationalize-0.0.1a1.dist-info/METADATA
+Filename: Python39/Lib/
 Comment: 
 
-Filename: Internationalize-0.0.1a1.dist-info/WHEEL
+Filename: Python39/Lib/site-packages/
 Comment: 
 
-Filename: Internationalize-0.0.1a1.dist-info/top_level.txt
+Filename: Python39/Lib/site-packages/internationalize/
 Comment: 
 
-Filename: Internationalize-0.0.1a1.dist-info/RECORD
+Filename: Python39/Lib/site-packages/Internationalize-0.0.2a2-py3.9.egg-info/
+Comment: 
+
+Filename: Python39/Lib/site-packages/internationalize/__pycache__/
+Comment: 
+
+Filename: Python39/Lib/site-packages/internationalize/configure.py
+Comment: 
+
+Filename: Python39/Lib/site-packages/internationalize/provider.py
+Comment: 
+
+Filename: Python39/Lib/site-packages/internationalize/__init__.py
+Comment: 
+
+Filename: Python39/Lib/site-packages/internationalize/__pycache__/configure.cpython-39.pyc
+Comment: 
+
+Filename: Python39/Lib/site-packages/internationalize/__pycache__/provider.cpython-39.pyc
+Comment: 
+
+Filename: Python39/Lib/site-packages/internationalize/__pycache__/__init__.cpython-39.pyc
+Comment: 
+
+Filename: Python39/Lib/site-packages/Internationalize-0.0.2a2-py3.9.egg-info/dependency_links.txt
+Comment: 
+
+Filename: Python39/Lib/site-packages/Internationalize-0.0.2a2-py3.9.egg-info/PKG-INFO
+Comment: 
+
+Filename: Python39/Lib/site-packages/Internationalize-0.0.2a2-py3.9.egg-info/SOURCES.txt
+Comment: 
+
+Filename: Python39/Lib/site-packages/Internationalize-0.0.2a2-py3.9.egg-info/top_level.txt
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## Comparing `Internationalize-0.0.1a1.dist-info/METADATA` & `Python39/Lib/site-packages/Internationalize-0.0.2a2-py3.9.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,70 @@
-Metadata-Version: 2.1
-Name: Internationalize
-Version: 0.0.1a1
-Summary: Helps to internationalize your application
-Home-page: https://github.com/smok-serwis/internationalize
-Author: Piotr Maślanka
-Author-email: pmaslanka@smok.co
-License: MIT License
-Keywords: i18n,internationalize
-Platform: posix
-Platform: win32
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: !=2.*,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
-Description-Content-Type: text/markdown; charset=UTF-8
-
-internationalize
-========
-[![PyPI version](https://badge.fury.io/py/internationalize.svg)](https://badge.fury.io/py/internationalize)
-[![PyPI](https://img.shields.io/pypi/pyversions/internationalize.svg)]()
-[![PyPI](https://img.shields.io/pypi/implementation/internationalize.svg)]()
-[![PyPI](https://img.shields.io/pypi/wheel/internationalize.svg)]()
-[![license](https://img.shields.io/github/license/mashape/apistatus.svg)]()
-
-A library to help you with internationalizing your application
-
-
+Metadata-Version: 2.1
+Name: Internationalize
+Version: 0.0.2a2
+Summary: Helps to internationalize your application
+Home-page: https://github.com/piotrmaslanka/internationalize
+Author: Piotr Maślanka
+Author-email: pmaslanka@smok.co
+License: MIT License
+Description: internationalize
+        ========
+        [![PyPI version](https://badge.fury.io/py/internationalize.svg)](https://badge.fury.io/py/internationalize)
+        [![PyPI](https://img.shields.io/pypi/pyversions/internationalize.svg)]()
+        [![PyPI](https://img.shields.io/pypi/implementation/internationalize.svg)]()
+        [![PyPI](https://img.shields.io/pypi/wheel/internationalize.svg)]()
+        [![license](https://img.shields.io/github/license/mashape/apistatus.svg)]()
+        
+        A library to help you with internationalizing your application.
+        [Here's a guide to using it](https://github.com/piotrmaslanka/Internationalize/wiki/How-to-use-Internationalize)
+        
+        Intro
+        -----
+        
+        While most Python internationalize libraries take an approach
+        with your providing a language and a keyword, and returning
+        a resembling string from an internal database, Internationalize 
+        takes a different approach.
+        
+        Internationalize asks you to provide a keyword, and then returning
+        a string containing a selection of the languages.
+        
+        Where you would configure the standard library with dictionary of mappings,
+        where each mapping would contain
+        
+        ```
+        configure_me({'hello': {'pl': 'Witaj'}, {'en': 'Hello'}})
+        pick_language('en')
+        ...
+        assert get_translation('hello') == 'Hello' 
+        ```
+        
+        Internationalize does the following:
+        
+        ```
+        configure_me({'hello': {'pl': 'Witaj'}, {'en': 'Hello'}})
+        ...
+        assert get_translation('hello') == {'pl': 'Witaj', {'en': Hello'}}
+        ```
+        
+        Which is super useful for handling certain applications that require those.
+        
+Keywords: i18n,internationalize
+Platform: posix
+Platform: win32
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: !=2.*,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
+Description-Content-Type: text/markdown; charset=UTF-8
```

