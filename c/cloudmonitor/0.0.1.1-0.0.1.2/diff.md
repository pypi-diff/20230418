# Comparing `tmp/cloudmonitor-0.0.1.1.tar.gz` & `tmp/cloudmonitor-0.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudmonitor-0.0.1.1.tar", last modified: Sun Apr 16 16:09:15 2023, max compression
+gzip compressed data, was "cloudmonitor-0.0.1.2.tar", last modified: Tue Apr 18 16:25:37 2023, max compression
```

## Comparing `cloudmonitor-0.0.1.1.tar` & `cloudmonitor-0.0.1.2.tar`

### file list

```diff
@@ -1,13 +1,24 @@
-drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-16 16:09:15.026480 cloudmonitor-0.0.1.1/
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      618 2023-04-16 16:09:15.022480 cloudmonitor-0.0.1.1/PKG-INFO
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-16 15:27:26.000000 cloudmonitor-0.0.1.1/README.md
-drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-16 16:09:15.022480 cloudmonitor-0.0.1.1/cloudmonitor/
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       23 2023-04-16 16:09:03.000000 cloudmonitor-0.0.1.1/cloudmonitor/__init__.py
-drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-16 16:09:15.022480 cloudmonitor-0.0.1.1/cloudmonitor.egg-info/
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      618 2023-04-16 16:09:15.000000 cloudmonitor-0.0.1.1/cloudmonitor.egg-info/PKG-INFO
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      222 2023-04-16 16:09:15.000000 cloudmonitor-0.0.1.1/cloudmonitor.egg-info/SOURCES.txt
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)        1 2023-04-16 16:09:15.000000 cloudmonitor-0.0.1.1/cloudmonitor.egg-info/dependency_links.txt
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       20 2023-04-16 16:09:15.000000 cloudmonitor-0.0.1.1/cloudmonitor.egg-info/requires.txt
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       13 2023-04-16 16:09:15.000000 cloudmonitor-0.0.1.1/cloudmonitor.egg-info/top_level.txt
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       38 2023-04-16 16:09:15.026480 cloudmonitor-0.0.1.1/setup.cfg
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2336 2023-04-16 16:07:57.000000 cloudmonitor-0.0.1.1/setup.py
+drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-18 16:25:37.000360 cloudmonitor-0.0.1.2/
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      618 2023-04-18 16:25:37.000360 cloudmonitor-0.0.1.2/PKG-INFO
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-16 15:27:26.000000 cloudmonitor-0.0.1.2/README.md
+drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-18 16:25:37.000360 cloudmonitor-0.0.1.2/cloudmonitor/
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       49 2023-04-18 16:24:18.000000 cloudmonitor-0.0.1.2/cloudmonitor/__init__.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       59 2023-04-18 16:06:41.000000 cloudmonitor-0.0.1.2/cloudmonitor/__main__.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     1578 2023-04-18 12:09:13.000000 cloudmonitor-0.0.1.2/cloudmonitor/config.py
+drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-18 16:25:37.000360 cloudmonitor-0.0.1.2/cloudmonitor/gpu/
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       43 2023-04-18 15:23:00.000000 cloudmonitor-0.0.1.2/cloudmonitor/gpu/__init__.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      277 2023-04-18 15:09:47.000000 cloudmonitor-0.0.1.2/cloudmonitor/gpu/define.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     1065 2023-04-18 16:00:25.000000 cloudmonitor-0.0.1.2/cloudmonitor/gpu/query.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2611 2023-04-18 16:06:26.000000 cloudmonitor-0.0.1.2/cloudmonitor/server.py
+drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-18 16:25:37.000360 cloudmonitor-0.0.1.2/cloudmonitor/ssh/
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       22 2023-04-18 15:28:12.000000 cloudmonitor-0.0.1.2/cloudmonitor/ssh/__init__.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      482 2023-04-18 15:00:34.000000 cloudmonitor-0.0.1.2/cloudmonitor/ssh/client.py
+drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-18 16:25:37.000360 cloudmonitor-0.0.1.2/cloudmonitor.egg-info/
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      618 2023-04-18 16:25:36.000000 cloudmonitor-0.0.1.2/cloudmonitor.egg-info/PKG-INFO
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      470 2023-04-18 16:25:36.000000 cloudmonitor-0.0.1.2/cloudmonitor.egg-info/SOURCES.txt
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)        1 2023-04-18 16:25:36.000000 cloudmonitor-0.0.1.2/cloudmonitor.egg-info/dependency_links.txt
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       52 2023-04-18 16:25:36.000000 cloudmonitor-0.0.1.2/cloudmonitor.egg-info/entry_points.txt
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       33 2023-04-18 16:25:36.000000 cloudmonitor-0.0.1.2/cloudmonitor.egg-info/requires.txt
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       13 2023-04-18 16:25:36.000000 cloudmonitor-0.0.1.2/cloudmonitor.egg-info/top_level.txt
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       38 2023-04-18 16:25:37.000360 cloudmonitor-0.0.1.2/setup.cfg
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2488 2023-04-18 15:58:03.000000 cloudmonitor-0.0.1.2/setup.py
```

### Comparing `cloudmonitor-0.0.1.1/PKG-INFO` & `cloudmonitor-0.0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudmonitor
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: A Web-GUI Monitor for Academic Linux Servers
 License: MIT Licence
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `cloudmonitor-0.0.1.1/cloudmonitor.egg-info/PKG-INFO` & `cloudmonitor-0.0.1.2/cloudmonitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudmonitor
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: A Web-GUI Monitor for Academic Linux Servers
 License: MIT Licence
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `cloudmonitor-0.0.1.1/setup.py` & `cloudmonitor-0.0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 if os.path.exists("MANIFEST"):
     os.remove("MANIFEST")
 
 # What packages are required for this module to be executed?
 # `estimator` may depend on other packages. In order to reduce dependencies, it is not written here.
 REQUIRED = [
     "numpy>=1.12.0, <1.24",
+    "flask>=2.2.2"
 ]
 
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
@@ -62,8 +63,13 @@
             "Operating System :: POSIX :: Linux",
             # "Operating System :: Microsoft :: Windows",
             # "Operating System :: MacOS",
             "Programming Language :: Python :: 3.6",
             "Programming Language :: Python :: 3.7",
             "Programming Language :: Python :: 3.8",
         ],
+        entry_points={
+            'console_scripts': [
+                'cloud-monitor = cloudmonitor:main',
+            ]
+        }
     )
```

