# Comparing `tmp/iloscar-0.2.7b0.tar.gz` & `tmp/iloscar-0.2.9b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iloscar-0.2.7b0.tar", last modified: Mon Apr 17 23:09:59 2023, max compression
+gzip compressed data, was "iloscar-0.2.9b0.tar", last modified: Tue Apr 18 00:43:17 2023, max compression
```

## Comparing `iloscar-0.2.7b0.tar` & `iloscar-0.2.9b0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-17 23:09:59.604171 iloscar-0.2.7b0/
--rw-r--r--   0 shihan     (504) staff       (20)    18344 2023-04-17 23:09:59.603933 iloscar-0.2.7b0/PKG-INFO
--rw-r--r--   0 shihan     (504) staff       (20)    17746 2023-04-17 20:16:31.000000 iloscar-0.2.7b0/README.md
-drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-17 23:09:59.600864 iloscar-0.2.7b0/iloscar/
--rw-r--r--   0 shihan     (504) staff       (20)      341 2023-04-05 02:45:38.000000 iloscar-0.2.7b0/iloscar/__init__.py
--rw-rw-r--   0 shihan     (504) staff       (20)     1941 2023-04-17 23:09:15.000000 iloscar-0.2.7b0/iloscar/app.py
-drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-17 23:09:59.602296 iloscar-0.2.7b0/iloscar/dat_y0/
--rw-r--r--   0 shihan     (504) staff       (20)     2957 2023-03-02 23:54:08.000000 iloscar-0.2.7b0/iloscar/dat_y0/petm_steady.dat
--rw-r--r--   0 shihan     (504) staff       (20)     1578 2023-03-03 22:13:41.000000 iloscar-0.2.7b0/iloscar/dat_y0/preind_steady.dat
--rw-rw-r--   0 shihan     (504) staff       (20)   106518 2023-04-17 20:14:07.000000 iloscar-0.2.7b0/iloscar/iLOSCAR_backend.py
-drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-17 23:09:59.603309 iloscar-0.2.7b0/iloscar/pages/
--rw-rw-r--   0 shihan     (504) staff       (20)     5797 2023-04-17 20:15:49.000000 iloscar-0.2.7b0/iloscar/pages/Function.py
--rw-rw-r--   0 shihan     (504) staff       (20)    26246 2023-04-17 20:37:12.000000 iloscar-0.2.7b0/iloscar/pages/forward.py
--rw-rw-r--   0 shihan     (504) staff       (20)      887 2023-04-17 20:15:56.000000 iloscar-0.2.7b0/iloscar/pages/home.py
--rw-rw-r--   0 shihan     (504) staff       (20)    46215 2023-04-17 20:49:42.000000 iloscar-0.2.7b0/iloscar/pages/inverse.py
--rw-r--r--   0 shihan     (504) staff       (20)     1357 2023-03-22 21:52:37.000000 iloscar-0.2.7b0/iloscar/style.py
-drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-17 23:09:59.601760 iloscar-0.2.7b0/iloscar.egg-info/
--rw-r--r--   0 shihan     (504) staff       (20)    18344 2023-04-17 23:09:59.000000 iloscar-0.2.7b0/iloscar.egg-info/PKG-INFO
--rw-r--r--   0 shihan     (504) staff       (20)      413 2023-04-17 23:09:59.000000 iloscar-0.2.7b0/iloscar.egg-info/SOURCES.txt
--rw-r--r--   0 shihan     (504) staff       (20)        1 2023-04-17 23:09:59.000000 iloscar-0.2.7b0/iloscar.egg-info/dependency_links.txt
--rw-r--r--   0 shihan     (504) staff       (20)      131 2023-04-17 23:09:59.000000 iloscar-0.2.7b0/iloscar.egg-info/requires.txt
--rw-r--r--   0 shihan     (504) staff       (20)       22 2023-04-17 23:09:59.000000 iloscar-0.2.7b0/iloscar.egg-info/top_level.txt
--rw-r--r--   0 shihan     (504) staff       (20)       38 2023-04-17 23:09:59.604230 iloscar-0.2.7b0/setup.cfg
--rw-r--r--   0 shihan     (504) staff       (20)     1451 2023-04-17 23:09:05.000000 iloscar-0.2.7b0/setup.py
+drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-18 00:43:17.988419 iloscar-0.2.9b0/
+-rw-r--r--   0 shihan     (504) staff       (20)    18344 2023-04-18 00:43:17.988078 iloscar-0.2.9b0/PKG-INFO
+-rw-r--r--   0 shihan     (504) staff       (20)    17746 2023-04-17 20:16:31.000000 iloscar-0.2.9b0/README.md
+drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-18 00:43:17.984687 iloscar-0.2.9b0/iloscar/
+-rw-r--r--   0 shihan     (504) staff       (20)      333 2023-04-18 00:38:17.000000 iloscar-0.2.9b0/iloscar/__init__.py
+-rw-rw-r--   0 shihan     (504) staff       (20)     1943 2023-04-18 00:40:26.000000 iloscar-0.2.9b0/iloscar/app.py
+drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-18 00:43:17.986341 iloscar-0.2.9b0/iloscar/dat_y0/
+-rw-r--r--   0 shihan     (504) staff       (20)     2957 2023-03-02 23:54:08.000000 iloscar-0.2.9b0/iloscar/dat_y0/petm_steady.dat
+-rw-r--r--   0 shihan     (504) staff       (20)     1578 2023-03-03 22:13:41.000000 iloscar-0.2.9b0/iloscar/dat_y0/preind_steady.dat
+-rw-rw-r--   0 shihan     (504) staff       (20)   106518 2023-04-17 20:14:07.000000 iloscar-0.2.9b0/iloscar/iLOSCAR_backend.py
+drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-18 00:43:17.987521 iloscar-0.2.9b0/iloscar/pages/
+-rw-rw-r--   0 shihan     (504) staff       (20)     5797 2023-04-17 20:15:49.000000 iloscar-0.2.9b0/iloscar/pages/Function.py
+-rw-rw-r--   0 shihan     (504) staff       (20)    26246 2023-04-17 20:37:12.000000 iloscar-0.2.9b0/iloscar/pages/forward.py
+-rw-rw-r--   0 shihan     (504) staff       (20)      887 2023-04-17 20:15:56.000000 iloscar-0.2.9b0/iloscar/pages/home.py
+-rw-rw-r--   0 shihan     (504) staff       (20)    46215 2023-04-17 20:49:42.000000 iloscar-0.2.9b0/iloscar/pages/inverse.py
+-rw-r--r--   0 shihan     (504) staff       (20)     1357 2023-03-22 21:52:37.000000 iloscar-0.2.9b0/iloscar/style.py
+drwxr-xr-x   0 shihan     (504) staff       (20)        0 2023-04-18 00:43:17.985763 iloscar-0.2.9b0/iloscar.egg-info/
+-rw-r--r--   0 shihan     (504) staff       (20)    18344 2023-04-18 00:43:17.000000 iloscar-0.2.9b0/iloscar.egg-info/PKG-INFO
+-rw-r--r--   0 shihan     (504) staff       (20)      413 2023-04-18 00:43:17.000000 iloscar-0.2.9b0/iloscar.egg-info/SOURCES.txt
+-rw-r--r--   0 shihan     (504) staff       (20)        1 2023-04-18 00:43:17.000000 iloscar-0.2.9b0/iloscar.egg-info/dependency_links.txt
+-rw-r--r--   0 shihan     (504) staff       (20)      131 2023-04-18 00:43:17.000000 iloscar-0.2.9b0/iloscar.egg-info/requires.txt
+-rw-r--r--   0 shihan     (504) staff       (20)       22 2023-04-18 00:43:17.000000 iloscar-0.2.9b0/iloscar.egg-info/top_level.txt
+-rw-r--r--   0 shihan     (504) staff       (20)       38 2023-04-18 00:43:17.988473 iloscar-0.2.9b0/setup.cfg
+-rw-r--r--   0 shihan     (504) staff       (20)     1451 2023-04-18 00:39:46.000000 iloscar-0.2.9b0/setup.py
```

### Comparing `iloscar-0.2.7b0/PKG-INFO` & `iloscar-0.2.9b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iloscar
-Version: 0.2.7b0
+Version: 0.2.9b0
 Summary: iLOSCAR
 Home-page: https://github.com/Shihan150/iloscar
 Author: Shihan Li
 Author-email: <shihan@tamu.edu>
 License: MIT
 Keywords: python,carbon cycle,model,paleoclimate,global warming,LOSCAR
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `iloscar-0.2.7b0/README.md` & `iloscar-0.2.9b0/README.md`

 * *Files identical despite different names*

### Comparing `iloscar-0.2.7b0/iloscar/app.py` & `iloscar-0.2.9b0/iloscar/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,8 +60,10 @@
                     [
                         dash.page_container
                     ], xs=8, sm=8, md=10, lg=10, xl=10, xxl=10)
             ]
         )
     ], fluid=True)
 
+
+
     app.run(debug=False, port = '7777')
```

### Comparing `iloscar-0.2.7b0/iloscar/dat_y0/petm_steady.dat` & `iloscar-0.2.9b0/iloscar/dat_y0/petm_steady.dat`

 * *Files identical despite different names*

### Comparing `iloscar-0.2.7b0/iloscar/dat_y0/preind_steady.dat` & `iloscar-0.2.9b0/iloscar/dat_y0/preind_steady.dat`

 * *Files identical despite different names*

### Comparing `iloscar-0.2.7b0/iloscar/iLOSCAR_backend.py` & `iloscar-0.2.9b0/iloscar/iLOSCAR_backend.py`

 * *Files identical despite different names*

### Comparing `iloscar-0.2.7b0/iloscar/pages/Function.py` & `iloscar-0.2.9b0/iloscar/pages/Function.py`

 * *Files identical despite different names*

### Comparing `iloscar-0.2.7b0/iloscar/pages/forward.py` & `iloscar-0.2.9b0/iloscar/pages/forward.py`

 * *Files identical despite different names*

### Comparing `iloscar-0.2.7b0/iloscar/pages/home.py` & `iloscar-0.2.9b0/iloscar/pages/home.py`

 * *Files identical despite different names*

### Comparing `iloscar-0.2.7b0/iloscar/pages/inverse.py` & `iloscar-0.2.9b0/iloscar/pages/inverse.py`

 * *Files identical despite different names*

### Comparing `iloscar-0.2.7b0/iloscar/style.py` & `iloscar-0.2.9b0/iloscar/style.py`

 * *Files identical despite different names*

### Comparing `iloscar-0.2.7b0/iloscar.egg-info/PKG-INFO` & `iloscar-0.2.9b0/iloscar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iloscar
-Version: 0.2.7b0
+Version: 0.2.9b0
 Summary: iLOSCAR
 Home-page: https://github.com/Shihan150/iloscar
 Author: Shihan Li
 Author-email: <shihan@tamu.edu>
 License: MIT
 Keywords: python,carbon cycle,model,paleoclimate,global warming,LOSCAR
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `iloscar-0.2.7b0/setup.py` & `iloscar-0.2.9b0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.7-beta'
+VERSION = '0.2.9-beta'
 DESCRIPTION = 'iLOSCAR'
 LONG_DESCRIPTION = 'A web-based interactive carbon cycle model, built upon the classic LOSCAR model.'
 
 # Setting up
 setup(
     name="iloscar",
     version=VERSION,
```

