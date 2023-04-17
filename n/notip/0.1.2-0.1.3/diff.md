# Comparing `tmp/notip-0.1.2.tar.gz` & `tmp/notip-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notip-0.1.2.tar", last modified: Mon Apr 17 13:20:55 2023, max compression
+gzip compressed data, was "notip-0.1.3.tar", last modified: Mon Apr 17 22:24:28 2023, max compression
```

## Comparing `notip-0.1.2.tar` & `notip-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 13:20:55.089073 notip-0.1.2/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1347 2023-04-17 13:20:55.089073 notip-0.1.2/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      848 2023-04-17 09:55:41.000000 notip-0.1.2/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 13:20:55.089073 notip-0.1.2/notip/
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-17 12:46:44.000000 notip-0.1.2/notip/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    26544 2022-07-01 17:10:03.000000 notip-0.1.2/notip/posthoc_fmri.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 13:20:55.089073 notip-0.1.2/notip.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1347 2023-04-17 13:20:55.000000 notip-0.1.2/notip.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      212 2023-04-17 13:20:55.000000 notip-0.1.2/notip.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-17 13:20:55.000000 notip-0.1.2/notip.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      108 2023-04-17 13:20:55.000000 notip-0.1.2/notip.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        6 2023-04-17 13:20:55.000000 notip-0.1.2/notip.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       79 2023-04-17 13:20:55.089073 notip-0.1.2/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)      976 2023-04-17 13:14:53.000000 notip-0.1.2/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 22:24:28.458430 notip-0.1.3/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1347 2023-04-17 22:24:28.458430 notip-0.1.3/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      848 2023-04-17 09:55:41.000000 notip-0.1.3/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 22:24:28.454430 notip-0.1.3/notip/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-17 12:46:44.000000 notip-0.1.3/notip/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    43762 2023-04-17 22:01:09.000000 notip-0.1.3/notip/posthoc_fmri.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-17 22:24:28.458430 notip-0.1.3/notip.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1347 2023-04-17 22:24:28.000000 notip-0.1.3/notip.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      212 2023-04-17 22:24:28.000000 notip-0.1.3/notip.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-17 22:24:28.000000 notip-0.1.3/notip.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      108 2023-04-17 22:24:28.000000 notip-0.1.3/notip.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        6 2023-04-17 22:24:28.000000 notip-0.1.3/notip.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       79 2023-04-17 22:24:28.458430 notip-0.1.3/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)      976 2023-04-17 22:20:43.000000 notip-0.1.3/setup.py
```

### Comparing `notip-0.1.2/PKG-INFO` & `notip-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notip
-Version: 0.1.2
+Version: 0.1.3
 Summary: Nonparametric True Discovery Proportion control for brain imaging
 Home-page: https://github.com/alexblnn/Notip
 Download-URL: https://github.com/alexblnn/Notip/releases/download/Notip_OHBM_v2/notip-0.1.2.tar.gz
 Author: Alexandre Blain
 Author-email: alexandre.blain@inria.fr
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `notip-0.1.2/README.md` & `notip-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `notip-0.1.2/notip.egg-info/PKG-INFO` & `notip-0.1.3/notip.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notip
-Version: 0.1.2
+Version: 0.1.3
 Summary: Nonparametric True Discovery Proportion control for brain imaging
 Home-page: https://github.com/alexblnn/Notip
 Download-URL: https://github.com/alexblnn/Notip/releases/download/Notip_OHBM_v2/notip-0.1.2.tar.gz
 Author: Alexandre Blain
 Author-email: alexandre.blain@inria.fr
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `notip-0.1.2/setup.py` & `notip-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 requirements = ["numpy>=1.15.0", "scipy>=1.0.0",
                 "joblib>=1.0.1", "scikit-learn>=0.22",
                 "nilearn","sanssouci","matplotlib",
                 "pandas", "joblib", "tqdm"]
 
 setup(
     name="notip",
-    version="0.1.2",
+    version="0.1.3",
     author="Alexandre Blain",
     author_email="alexandre.blain@inria.fr",
     description="Nonparametric True Discovery Proportion control for brain imaging",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/alexblnn/Notip",
     download_url="https://github.com/alexblnn/Notip/releases/download/Notip_OHBM_v2/notip-0.1.2.tar.gz",
```

