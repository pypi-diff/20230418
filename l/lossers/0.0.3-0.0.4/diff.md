# Comparing `tmp/lossers-0.0.3.tar.gz` & `tmp/lossers-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lossers-0.0.3.tar", last modified: Tue Apr 18 11:41:24 2023, max compression
+gzip compressed data, was "lossers-0.0.4.tar", last modified: Tue Apr 18 15:15:55 2023, max compression
```

## Comparing `lossers-0.0.3.tar` & `lossers-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:41:24.337189 lossers-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-18 11:41:13.000000 lossers-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-18 11:41:24.337189 lossers-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-18 11:41:13.000000 lossers-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:41:24.337189 lossers-0.0.3/lossers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:41:13.000000 lossers-0.0.3/lossers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-18 11:41:13.000000 lossers-0.0.3/lossers/clip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:41:24.337189 lossers-0.0.3/lossers/lpips/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 11:41:13.000000 lossers-0.0.3/lossers/lpips/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-18 11:41:13.000000 lossers-0.0.3/lossers/lpips/lpips.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-18 11:41:13.000000 lossers-0.0.3/lossers/lpips/pretrained_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-18 11:41:13.000000 lossers-0.0.3/lossers/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-18 11:41:13.000000 lossers-0.0.3/lossers/ssim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:41:24.337189 lossers-0.0.3/lossers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-18 11:41:24.000000 lossers-0.0.3/lossers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-18 11:41:24.000000 lossers-0.0.3/lossers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 11:41:24.000000 lossers-0.0.3/lossers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 11:41:24.000000 lossers-0.0.3/lossers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 11:41:24.337189 lossers-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-18 11:41:13.000000 lossers-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:15:55.347069 lossers-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-18 15:15:45.000000 lossers-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-18 15:15:55.347069 lossers-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-18 15:15:45.000000 lossers-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:15:55.343069 lossers-0.0.4/lossers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:15:45.000000 lossers-0.0.4/lossers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-18 15:15:45.000000 lossers-0.0.4/lossers/clip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:15:55.347069 lossers-0.0.4/lossers/lpips/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 15:15:45.000000 lossers-0.0.4/lossers/lpips/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-18 15:15:45.000000 lossers-0.0.4/lossers/lpips/lpips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-18 15:15:45.000000 lossers-0.0.4/lossers/lpips/pretrained_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-04-18 15:15:45.000000 lossers-0.0.4/lossers/lpips/vgg_v0.1.pth
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-18 15:15:45.000000 lossers-0.0.4/lossers/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-18 15:15:45.000000 lossers-0.0.4/lossers/ssim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:15:55.347069 lossers-0.0.4/lossers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-18 15:15:55.000000 lossers-0.0.4/lossers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-18 15:15:55.000000 lossers-0.0.4/lossers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:15:55.000000 lossers-0.0.4/lossers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 15:15:55.000000 lossers-0.0.4/lossers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 15:15:55.347069 lossers-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-18 15:15:45.000000 lossers-0.0.4/setup.py
```

### Comparing `lossers-0.0.3/LICENSE` & `lossers-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lossers-0.0.3/PKG-INFO` & `lossers-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 Metadata-Version: 2.1
 Name: lossers
-Version: 0.0.3
-Summary: ML Loss Function
+Version: 0.0.4
+Summary: ML/DL Loss Function
 Home-page: https://github.com/JiauZhang/lossers
 Author: JiauZhang
 Author-email: jiauzhang@163.com
 License: MIT
 Keywords: artificial intelligence,loss function,deep learning
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+
+
+```shell
+pip install lossers
+# or install from source
+pip install git+https://github.com/JiauZhang/lossers.git
+```
```

### Comparing `lossers-0.0.3/lossers/lpips/lpips.py` & `lossers-0.0.4/lossers/lpips/lpips.py`

 * *Files identical despite different names*

### Comparing `lossers-0.0.3/lossers/lpips/pretrained_model.py` & `lossers-0.0.4/lossers/lpips/pretrained_model.py`

 * *Files identical despite different names*

### Comparing `lossers-0.0.3/lossers/ssim.py` & `lossers-0.0.4/lossers/ssim.py`

 * *Files identical despite different names*

### Comparing `lossers-0.0.3/lossers.egg-info/PKG-INFO` & `lossers-0.0.4/lossers.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 Metadata-Version: 2.1
 Name: lossers
-Version: 0.0.3
-Summary: ML Loss Function
+Version: 0.0.4
+Summary: ML/DL Loss Function
 Home-page: https://github.com/JiauZhang/lossers
 Author: JiauZhang
 Author-email: jiauzhang@163.com
 License: MIT
 Keywords: artificial intelligence,loss function,deep learning
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+
+
+```shell
+pip install lossers
+# or install from source
+pip install git+https://github.com/JiauZhang/lossers.git
+```
```

