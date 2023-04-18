# Comparing `tmp/Slim-TPCA-0.0.4.tar.gz` & `tmp/Slim-TPCA-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slim-TPCA-0.0.4.tar", last modified: Tue Apr 18 06:40:56 2023, max compression
+gzip compressed data, was "Slim-TPCA-0.0.5.tar", last modified: Tue Apr 18 06:58:26 2023, max compression
```

## Comparing `Slim-TPCA-0.0.4.tar` & `Slim-TPCA-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 wangjun   (1000) wangjun   (1000)        0 2023-04-18 06:40:56.185391 Slim-TPCA-0.0.4/
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     1091 2022-11-08 05:40:40.000000 Slim-TPCA-0.0.4/LICENSE
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     3346 2023-04-18 06:40:56.185391 Slim-TPCA-0.0.4/PKG-INFO
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     2618 2022-11-08 05:40:40.000000 Slim-TPCA-0.0.4/README.md
-drwxrwxr-x   0 wangjun   (1000) wangjun   (1000)        0 2023-04-18 06:40:56.185391 Slim-TPCA-0.0.4/Slim_TPCA.egg-info/
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     3346 2023-04-18 06:40:56.000000 Slim-TPCA-0.0.4/Slim_TPCA.egg-info/PKG-INFO
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)      205 2023-04-18 06:40:56.000000 Slim-TPCA-0.0.4/Slim_TPCA.egg-info/SOURCES.txt
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)        1 2023-04-18 06:40:56.000000 Slim-TPCA-0.0.4/Slim_TPCA.egg-info/dependency_links.txt
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)       95 2023-04-18 06:40:56.000000 Slim-TPCA-0.0.4/Slim_TPCA.egg-info/requires.txt
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)        1 2023-04-18 06:40:56.000000 Slim-TPCA-0.0.4/Slim_TPCA.egg-info/top_level.txt
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)      652 2023-04-18 06:34:47.000000 Slim-TPCA-0.0.4/pyproject.toml
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)       38 2023-04-18 06:40:56.185391 Slim-TPCA-0.0.4/setup.cfg
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     1086 2023-04-18 06:34:56.000000 Slim-TPCA-0.0.4/setup.py
+drwxrwxr-x   0 wangjun   (1000) wangjun   (1000)        0 2023-04-18 06:58:26.647997 Slim-TPCA-0.0.5/
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     1091 2022-11-08 05:40:40.000000 Slim-TPCA-0.0.5/LICENSE
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     3346 2023-04-18 06:58:26.643998 Slim-TPCA-0.0.5/PKG-INFO
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     2618 2022-11-08 05:40:40.000000 Slim-TPCA-0.0.5/README.md
+drwxrwxr-x   0 wangjun   (1000) wangjun   (1000)        0 2023-04-18 06:58:26.643998 Slim-TPCA-0.0.5/Slim_TPCA.egg-info/
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     3346 2023-04-18 06:58:26.000000 Slim-TPCA-0.0.5/Slim_TPCA.egg-info/PKG-INFO
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)      205 2023-04-18 06:58:26.000000 Slim-TPCA-0.0.5/Slim_TPCA.egg-info/SOURCES.txt
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)        1 2023-04-18 06:58:26.000000 Slim-TPCA-0.0.5/Slim_TPCA.egg-info/dependency_links.txt
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)       95 2023-04-18 06:58:26.000000 Slim-TPCA-0.0.5/Slim_TPCA.egg-info/requires.txt
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)        1 2023-04-18 06:58:26.000000 Slim-TPCA-0.0.5/Slim_TPCA.egg-info/top_level.txt
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)      652 2023-04-18 06:57:56.000000 Slim-TPCA-0.0.5/pyproject.toml
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)       38 2023-04-18 06:58:26.647997 Slim-TPCA-0.0.5/setup.cfg
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     1086 2023-04-18 06:58:07.000000 Slim-TPCA-0.0.5/setup.py
```

### Comparing `Slim-TPCA-0.0.4/LICENSE` & `Slim-TPCA-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Slim-TPCA-0.0.4/PKG-INFO` & `Slim-TPCA-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Slim-TPCA
-Version: 0.0.4
+Version: 0.0.5
 Summary: Slim-TPCA: a python package to expediate functional characterization of existing and newly identified protein complexes by optimizing existing TPCA algorithm implementations
 Home-page: https://github.com/wangjun258/Slim_TPCA
 Author: Siyuan Sun, Jun Wang
 Author-email: Siyuan Sun <11930100@mail.sustech.edu.cn>
 Project-URL: Homepage, https://github.com/pypa/Slim_TPCA
 Project-URL: Bug Tracker, https://github.com/pypa/Slim_TPCA/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Slim-TPCA-0.0.4/README.md` & `Slim-TPCA-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `Slim-TPCA-0.0.4/Slim_TPCA.egg-info/PKG-INFO` & `Slim-TPCA-0.0.5/Slim_TPCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Slim-TPCA
-Version: 0.0.4
+Version: 0.0.5
 Summary: Slim-TPCA: a python package to expediate functional characterization of existing and newly identified protein complexes by optimizing existing TPCA algorithm implementations
 Home-page: https://github.com/wangjun258/Slim_TPCA
 Author: Siyuan Sun, Jun Wang
 Author-email: Siyuan Sun <11930100@mail.sustech.edu.cn>
 Project-URL: Homepage, https://github.com/pypa/Slim_TPCA
 Project-URL: Bug Tracker, https://github.com/pypa/Slim_TPCA/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Slim-TPCA-0.0.4/pyproject.toml` & `Slim-TPCA-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Slim-TPCA"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Siyuan Sun", email="11930100@mail.sustech.edu.cn" },
 ]
 description = "Slim-TPCA: a python package to expediate functional characterization of existing and newly identified protein complexes by optimizing existing TPCA algorithm implementations"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `Slim-TPCA-0.0.4/setup.py` & `Slim-TPCA-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Slim_TPCA',
-    version='0.0.4',
+    version='0.0.5',
     description='Slim-TPCA package is a python package which requires python version higher than 3.7 to work. Slim-TPCA has been optimised based on the TPCA method published in 2018. By using fewer temperature points, Slim-TPCA can reduce the volume of samples required, eliminate the batch effect in multiplex mass spectrometry experiments, and greatly shorten the calculation time required. In the Slim-TPCA package, users can perform data pre-processing, graph ROC plots to determine the ability of the data to predict protein interactions, calculate the TPCA signatures of the complexes and dynamic modulations of the complexes',
     url='https://github.com/wangjun258/Slim_TPCA',
     author='Siyuan Sun, Jun Wang',
     author_email='11930100@mail.sustech.edu.cn',
     packages=find_packages(),
     install_requires=[
         'numpy>=1.22.4',
```

