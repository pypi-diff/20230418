# Comparing `tmp/extr-ds-0.0.7.tar.gz` & `tmp/extr-ds-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extr-ds-0.0.7.tar", last modified: Tue Apr 18 10:03:31 2023, max compression
+gzip compressed data, was "extr-ds-0.0.8.tar", last modified: Tue Apr 18 12:37:23 2023, max compression
```

## Comparing `extr-ds-0.0.7.tar` & `extr-ds-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 10:03:31.438516 extr-ds-0.0.7/
--rw-rw-rw-   0        0        0     4025 2023-04-18 10:03:31.436303 extr-ds-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2846 2023-04-18 10:02:42.000000 extr-ds-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-04-18 10:03:31.443818 extr-ds-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      607 2023-04-18 09:58:31.000000 extr-ds-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:03:31.266364 extr-ds-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-18 10:03:31.304103 extr-ds-0.0.7/src/extr_ds/
--rw-rw-rw-   0        0        0       27 2023-04-15 12:51:37.000000 extr-ds-0.0.7/src/extr_ds/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:03:31.425333 extr-ds-0.0.7/src/extr_ds/labelers/
--rw-rw-rw-   0        0        0       68 2023-04-16 10:14:54.000000 extr-ds-0.0.7/src/extr_ds/labelers/__init__.py
--rw-rw-rw-   0        0        0     1634 2023-04-18 10:03:06.000000 extr-ds-0.0.7/src/extr_ds/labelers/iob.py
--rw-rw-rw-   0        0        0     3885 2023-04-18 10:00:03.000000 extr-ds-0.0.7/src/extr_ds/labelers/relation.py
--rw-rw-rw-   0        0        0      461 2023-04-18 09:59:18.000000 extr-ds-0.0.7/src/extr_ds/models.py
--rw-rw-rw-   0        0        0     1718 2023-04-17 21:01:45.000000 extr-ds-0.0.7/src/extr_ds/validators.py
-drwxrwxrwx   0        0        0        0 2023-04-18 10:03:31.392208 extr-ds-0.0.7/src/extr_ds.egg-info/
--rw-rw-rw-   0        0        0     4025 2023-04-18 10:03:30.000000 extr-ds-0.0.7/src/extr_ds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2023-04-18 10:03:31.000000 extr-ds-0.0.7/src/extr_ds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 10:03:30.000000 extr-ds-0.0.7/src/extr_ds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-18 10:03:30.000000 extr-ds-0.0.7/src/extr_ds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-18 10:03:30.000000 extr-ds-0.0.7/src/extr_ds.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 12:37:23.907924 extr-ds-0.0.8/
+-rw-rw-rw-   0        0        0     4025 2023-04-18 12:37:23.903846 extr-ds-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2846 2023-04-18 10:02:42.000000 extr-ds-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-18 12:37:23.913226 extr-ds-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      608 2023-04-18 12:37:10.000000 extr-ds-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 12:37:23.714591 extr-ds-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-04-18 12:37:23.751851 extr-ds-0.0.8/src/extr_ds/
+-rw-rw-rw-   0        0        0       27 2023-04-15 12:51:37.000000 extr-ds-0.0.8/src/extr_ds/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 12:37:23.895063 extr-ds-0.0.8/src/extr_ds/labelers/
+-rw-rw-rw-   0        0        0       68 2023-04-16 10:14:54.000000 extr-ds-0.0.8/src/extr_ds/labelers/__init__.py
+-rw-rw-rw-   0        0        0     1634 2023-04-18 10:03:06.000000 extr-ds-0.0.8/src/extr_ds/labelers/iob.py
+-rw-rw-rw-   0        0        0     3608 2023-04-18 12:35:59.000000 extr-ds-0.0.8/src/extr_ds/labelers/relation.py
+-rw-rw-rw-   0        0        0      461 2023-04-18 09:59:18.000000 extr-ds-0.0.8/src/extr_ds/models.py
+-rw-rw-rw-   0        0        0     1718 2023-04-17 21:01:45.000000 extr-ds-0.0.8/src/extr_ds/validators.py
+drwxrwxrwx   0        0        0        0 2023-04-18 12:37:23.868792 extr-ds-0.0.8/src/extr_ds.egg-info/
+-rw-rw-rw-   0        0        0     4025 2023-04-18 12:37:23.000000 extr-ds-0.0.8/src/extr_ds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-04-18 12:37:23.000000 extr-ds-0.0.8/src/extr_ds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 12:37:23.000000 extr-ds-0.0.8/src/extr_ds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-18 12:37:23.000000 extr-ds-0.0.8/src/extr_ds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-18 12:37:23.000000 extr-ds-0.0.8/src/extr_ds.egg-info/top_level.txt
```

### Comparing `extr-ds-0.0.7/PKG-INFO` & `extr-ds-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extr-ds
-Version: 0.0.7
+Version: 0.0.8
 Summary: Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
 Home-page: https://github.com/dpasse/extr-ds
 License: UNKNOWN
 Description: # extr-ds
         > Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
         
         <br />
```

### Comparing `extr-ds-0.0.7/README.md` & `extr-ds-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `extr-ds-0.0.7/setup.py` & `extr-ds-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='extr-ds',
-    version='0.0.7',
+    version='0.0.8',
     keywords='',
     description='Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.',
     packages=setuptools.find_packages('src'),
     package_dir={'': 'src'},
     install_requires=[
-        'extr==0.0.8'
+        'extr==0.0.10'
     ],
     url='https://github.com/dpasse/extr-ds',
     long_description=long_description,
     long_description_content_type='text/markdown',
 )
```

### Comparing `extr-ds-0.0.7/src/extr_ds/labelers/iob.py` & `extr-ds-0.0.8/src/extr_ds/labelers/iob.py`

 * *Files identical despite different names*

### Comparing `extr-ds-0.0.7/src/extr_ds/validators.py` & `extr-ds-0.0.8/src/extr_ds/validators.py`

 * *Files identical despite different names*

### Comparing `extr-ds-0.0.7/src/extr_ds.egg-info/PKG-INFO` & `extr-ds-0.0.8/src/extr_ds.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extr-ds
-Version: 0.0.7
+Version: 0.0.8
 Summary: Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
 Home-page: https://github.com/dpasse/extr-ds
 License: UNKNOWN
 Description: # extr-ds
         > Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
         
         <br />
```

