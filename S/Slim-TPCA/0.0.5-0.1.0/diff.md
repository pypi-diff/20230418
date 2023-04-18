# Comparing `tmp/Slim-TPCA-0.0.5.tar.gz` & `tmp/Slim-TPCA-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slim-TPCA-0.0.5.tar", last modified: Tue Apr 18 06:58:26 2023, max compression
+gzip compressed data, was "Slim-TPCA-0.1.0.tar", last modified: Tue Apr 18 07:12:02 2023, max compression
```

## Comparing `Slim-TPCA-0.0.5.tar` & `Slim-TPCA-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxr-x   0 wangjun   (1000) wangjun   (1000)        0 2023-04-18 06:58:26.647997 Slim-TPCA-0.0.5/
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     1091 2022-11-08 05:40:40.000000 Slim-TPCA-0.0.5/LICENSE
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     3346 2023-04-18 06:58:26.643998 Slim-TPCA-0.0.5/PKG-INFO
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     2618 2022-11-08 05:40:40.000000 Slim-TPCA-0.0.5/README.md
-drwxrwxr-x   0 wangjun   (1000) wangjun   (1000)        0 2023-04-18 06:58:26.643998 Slim-TPCA-0.0.5/Slim_TPCA.egg-info/
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     3346 2023-04-18 06:58:26.000000 Slim-TPCA-0.0.5/Slim_TPCA.egg-info/PKG-INFO
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)      205 2023-04-18 06:58:26.000000 Slim-TPCA-0.0.5/Slim_TPCA.egg-info/SOURCES.txt
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)        1 2023-04-18 06:58:26.000000 Slim-TPCA-0.0.5/Slim_TPCA.egg-info/dependency_links.txt
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)       95 2023-04-18 06:58:26.000000 Slim-TPCA-0.0.5/Slim_TPCA.egg-info/requires.txt
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)        1 2023-04-18 06:58:26.000000 Slim-TPCA-0.0.5/Slim_TPCA.egg-info/top_level.txt
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)      652 2023-04-18 06:57:56.000000 Slim-TPCA-0.0.5/pyproject.toml
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)       38 2023-04-18 06:58:26.647997 Slim-TPCA-0.0.5/setup.cfg
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     1086 2023-04-18 06:58:07.000000 Slim-TPCA-0.0.5/setup.py
+drwxrwxr-x   0 wangjun   (1000) wangjun   (1000)        0 2023-04-18 07:12:02.260323 Slim-TPCA-0.1.0/
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     1091 2022-11-08 05:40:40.000000 Slim-TPCA-0.1.0/LICENSE
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     3266 2023-04-18 07:12:02.260323 Slim-TPCA-0.1.0/PKG-INFO
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     2618 2022-11-08 05:40:40.000000 Slim-TPCA-0.1.0/README.md
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)      652 2023-04-18 07:11:45.000000 Slim-TPCA-0.1.0/pyproject.toml
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)       38 2023-04-18 07:12:02.260323 Slim-TPCA-0.1.0/setup.cfg
+drwxrwxr-x   0 wangjun   (1000) wangjun   (1000)        0 2023-04-18 07:12:02.260323 Slim-TPCA-0.1.0/src/
+drwxrwxr-x   0 wangjun   (1000) wangjun   (1000)        0 2023-04-18 07:12:02.260323 Slim-TPCA-0.1.0/src/Slim_TPCA/
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)    12827 2022-11-08 05:40:40.000000 Slim-TPCA-0.1.0/src/Slim_TPCA/Slim_TPCA.py
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)        0 2022-11-08 05:40:40.000000 Slim-TPCA-0.1.0/src/Slim_TPCA/__init__.py
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     1086 2023-04-18 07:11:19.000000 Slim-TPCA-0.1.0/src/Slim_TPCA/setup.py
+drwxrwxr-x   0 wangjun   (1000) wangjun   (1000)        0 2023-04-18 07:12:02.260323 Slim-TPCA-0.1.0/src/Slim_TPCA.egg-info/
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     3266 2023-04-18 07:12:02.000000 Slim-TPCA-0.1.0/src/Slim_TPCA.egg-info/PKG-INFO
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)      256 2023-04-18 07:12:02.000000 Slim-TPCA-0.1.0/src/Slim_TPCA.egg-info/SOURCES.txt
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)        1 2023-04-18 07:12:02.000000 Slim-TPCA-0.1.0/src/Slim_TPCA.egg-info/dependency_links.txt
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)       10 2023-04-18 07:12:02.000000 Slim-TPCA-0.1.0/src/Slim_TPCA.egg-info/top_level.txt
```

### Comparing `Slim-TPCA-0.0.5/LICENSE` & `Slim-TPCA-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Slim-TPCA-0.0.5/PKG-INFO` & `Slim-TPCA-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: Slim-TPCA
-Version: 0.0.5
+Version: 0.1.0
 Summary: Slim-TPCA: a python package to expediate functional characterization of existing and newly identified protein complexes by optimizing existing TPCA algorithm implementations
-Home-page: https://github.com/wangjun258/Slim_TPCA
-Author: Siyuan Sun, Jun Wang
 Author-email: Siyuan Sun <11930100@mail.sustech.edu.cn>
 Project-URL: Homepage, https://github.com/pypa/Slim_TPCA
 Project-URL: Bug Tracker, https://github.com/pypa/Slim_TPCA/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `Slim-TPCA-0.0.5/README.md` & `Slim-TPCA-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `Slim-TPCA-0.0.5/Slim_TPCA.egg-info/PKG-INFO` & `Slim-TPCA-0.1.0/src/Slim_TPCA.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: Slim-TPCA
-Version: 0.0.5
+Version: 0.1.0
 Summary: Slim-TPCA: a python package to expediate functional characterization of existing and newly identified protein complexes by optimizing existing TPCA algorithm implementations
-Home-page: https://github.com/wangjun258/Slim_TPCA
-Author: Siyuan Sun, Jun Wang
 Author-email: Siyuan Sun <11930100@mail.sustech.edu.cn>
 Project-URL: Homepage, https://github.com/pypa/Slim_TPCA
 Project-URL: Bug Tracker, https://github.com/pypa/Slim_TPCA/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `Slim-TPCA-0.0.5/pyproject.toml` & `Slim-TPCA-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Slim-TPCA"
-version = "0.0.5"
+version = "0.1.0"
 authors = [
   { name="Siyuan Sun", email="11930100@mail.sustech.edu.cn" },
 ]
 description = "Slim-TPCA: a python package to expediate functional characterization of existing and newly identified protein complexes by optimizing existing TPCA algorithm implementations"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `Slim-TPCA-0.0.5/setup.py` & `Slim-TPCA-0.1.0/src/Slim_TPCA/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Slim_TPCA',
-    version='0.0.5',
+    version='0.1.0',
     description='Slim-TPCA package is a python package which requires python version higher than 3.7 to work. Slim-TPCA has been optimised based on the TPCA method published in 2018. By using fewer temperature points, Slim-TPCA can reduce the volume of samples required, eliminate the batch effect in multiplex mass spectrometry experiments, and greatly shorten the calculation time required. In the Slim-TPCA package, users can perform data pre-processing, graph ROC plots to determine the ability of the data to predict protein interactions, calculate the TPCA signatures of the complexes and dynamic modulations of the complexes',
     url='https://github.com/wangjun258/Slim_TPCA',
     author='Siyuan Sun, Jun Wang',
     author_email='11930100@mail.sustech.edu.cn',
     packages=find_packages(),
     install_requires=[
         'numpy>=1.22.4',
```

