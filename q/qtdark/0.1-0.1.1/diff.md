# Comparing `tmp/qtdark-0.1.tar.gz` & `tmp/qtdark-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtdark-0.1.tar", last modified: Tue Apr 18 13:20:16 2023, max compression
+gzip compressed data, was "qtdark-0.1.1.tar", last modified: Tue Apr 18 13:59:15 2023, max compression
```

## Comparing `qtdark-0.1.tar` & `qtdark-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 13:20:16.882358 qtdark-0.1/
--rw-rw-rw-   0        0        0     1097 2023-04-18 12:59:58.000000 qtdark-0.1/LICENSE
--rw-rw-rw-   0        0        0      558 2023-04-18 13:20:16.882358 qtdark-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        8 2023-04-18 12:59:58.000000 qtdark-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 13:20:16.875377 qtdark-0.1/qtdark/
--rw-rw-rw-   0        0        0      253 2023-04-18 13:13:53.000000 qtdark-0.1/qtdark/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 13:20:16.881361 qtdark-0.1/qtdark.egg-info/
--rw-rw-rw-   0        0        0      558 2023-04-18 13:20:16.000000 qtdark-0.1/qtdark.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-04-18 13:20:16.000000 qtdark-0.1/qtdark.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 13:20:16.000000 qtdark-0.1/qtdark.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-18 13:20:16.000000 qtdark-0.1/qtdark.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 13:20:16.000000 qtdark-0.1/qtdark.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 13:20:16.883355 qtdark-0.1/setup.cfg
--rw-rw-rw-   0        0        0      663 2023-04-18 13:17:32.000000 qtdark-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 13:59:15.251944 qtdark-0.1.1/
+-rw-rw-rw-   0        0        0     1097 2023-04-18 12:59:58.000000 qtdark-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      560 2023-04-18 13:59:15.250947 qtdark-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        8 2023-04-18 12:59:58.000000 qtdark-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 13:59:15.249949 qtdark-0.1.1/qtdark.egg-info/
+-rw-rw-rw-   0        0        0      560 2023-04-18 13:59:15.000000 qtdark-0.1.1/qtdark.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2023-04-18 13:59:15.000000 qtdark-0.1.1/qtdark.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 13:59:15.000000 qtdark-0.1.1/qtdark.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-18 13:59:15.000000 qtdark-0.1.1/qtdark.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 13:59:15.000000 qtdark-0.1.1/qtdark.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 13:59:15.251944 qtdark-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      665 2023-04-18 13:59:08.000000 qtdark-0.1.1/setup.py
```

### Comparing `qtdark-0.1/LICENSE` & `qtdark-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qtdark-0.1/PKG-INFO` & `qtdark-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: qtdark
-Version: 0.1
+Version: 0.1.1
 Summary: UNKNOWN
 Home-page: https://github.com/nguyenvantat1182002/qtdark
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `qtdark-0.1/qtdark.egg-info/PKG-INFO` & `qtdark-0.1.1/qtdark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: qtdark
-Version: 0.1
+Version: 0.1.1
 Summary: UNKNOWN
 Home-page: https://github.com/nguyenvantat1182002/qtdark
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `qtdark-0.1/setup.py` & `qtdark-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='qtdark',
-    version='0.1',
+    version='0.1.1',
     author='Tat Nguyen Van',
     author_email='nguyenvantat1182002@gmail.com',
     url='https://github.com/nguyenvantat1182002/qtdark',
     packages=find_packages(),
     install_requires=[
         'pyqt5-tools',
         'pyqt5'
```

