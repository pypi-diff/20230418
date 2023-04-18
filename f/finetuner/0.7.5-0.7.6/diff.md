# Comparing `tmp/finetuner-0.7.5.tar.gz` & `tmp/finetuner-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finetuner-0.7.5.tar", last modified: Fri Apr 14 07:39:18 2023, max compression
+gzip compressed data, was "finetuner-0.7.6.tar", last modified: Tue Apr 18 15:27:57 2023, max compression
```

## Comparing `finetuner-0.7.5.tar` & `finetuner-0.7.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:39:18.047494 finetuner-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-04-14 07:39:08.000000 finetuner-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-14 07:39:08.000000 finetuner-0.7.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-04-14 07:39:18.047494 finetuner-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-04-14 07:39:08.000000 finetuner-0.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:39:18.043494 finetuner-0.7.5/finetuner/
--rw-r--r--   0 runner    (1001) docker     (123)    23608 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:39:18.047494 finetuner-0.7.5/finetuner/client/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/client/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/client/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/excepts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/finetuner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/hubble.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:39:18.043494 finetuner-0.7.5/finetuner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-04-14 07:39:17.000000 finetuner-0.7.5/finetuner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-14 07:39:17.000000 finetuner-0.7.5/finetuner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 07:39:17.000000 finetuner-0.7.5/finetuner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 07:39:17.000000 finetuner-0.7.5/finetuner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-14 07:39:17.000000 finetuner-0.7.5/finetuner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 07:39:17.000000 finetuner-0.7.5/finetuner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-14 07:39:08.000000 finetuner-0.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-14 07:39:18.047494 finetuner-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-14 07:39:08.000000 finetuner-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:27:57.118135 finetuner-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-04-18 15:27:27.000000 finetuner-0.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-18 15:27:27.000000 finetuner-0.7.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-04-18 15:27:57.118135 finetuner-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-04-18 15:27:27.000000 finetuner-0.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:27:57.118135 finetuner-0.7.6/finetuner/
+-rw-r--r--   0 runner    (1001) docker     (123)    23608 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:27:57.118135 finetuner-0.7.6/finetuner/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/client/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/excepts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/finetuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/hubble.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-04-18 15:27:27.000000 finetuner-0.7.6/finetuner/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:27:57.118135 finetuner-0.7.6/finetuner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-04-18 15:27:55.000000 finetuner-0.7.6/finetuner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-18 15:27:57.000000 finetuner-0.7.6/finetuner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:27:55.000000 finetuner-0.7.6/finetuner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:27:55.000000 finetuner-0.7.6/finetuner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-18 15:27:55.000000 finetuner-0.7.6/finetuner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 15:27:55.000000 finetuner-0.7.6/finetuner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-18 15:27:27.000000 finetuner-0.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-18 15:27:57.118135 finetuner-0.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-18 15:27:27.000000 finetuner-0.7.6/setup.py
```

### Comparing `finetuner-0.7.5/LICENSE` & `finetuner-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.5/PKG-INFO` & `finetuner-0.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finetuner
-Version: 0.7.5
+Version: 0.7.6
 Summary: Task-oriented finetuning for better embeddings on neural search.
 Home-page: https://github.com/jina-ai/finetuner/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/finetuner/tags
 Project-URL: Documentation, https://finetuner.jina.ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: finetuner Version: 0.7.5 Summary: Task-oriented
+Metadata-Version: 2.1 Name: finetuner Version: 0.7.6 Summary: Task-oriented
 finetuning for better embeddings on neural search. Home-page: https://
 github.com/jina-ai/finetuner/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/finetuner/tags
 Project-URL: Documentation, https://finetuner.jina.ai Project-URL: Source,
 https://github.com/jina-ai/finetuner/ Project-URL: Tracker, https://github.com/
 jina-ai/finetuner/issues Description:
```

### Comparing `finetuner-0.7.5/README.md` & `finetuner-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.5/finetuner/__init__.py` & `finetuner-0.7.6/finetuner/__init__.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.5/finetuner/client/base.py` & `finetuner-0.7.6/finetuner/client/base.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.5/finetuner/client/client.py` & `finetuner-0.7.6/finetuner/client/client.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.5/finetuner/client/session.py` & `finetuner-0.7.6/finetuner/client/session.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.5/finetuner/console.py` & `finetuner-0.7.6/finetuner/console.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.5/finetuner/constants.py` & `finetuner-0.7.6/finetuner/constants.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.5/finetuner/data.py` & `finetuner-0.7.6/finetuner/data.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.5/finetuner/experiment.py` & `finetuner-0.7.6/finetuner/experiment.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.5/finetuner/finetuner.py` & `finetuner-0.7.6/finetuner/finetuner.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.5/finetuner/hubble.py` & `finetuner-0.7.6/finetuner/hubble.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.5/finetuner/model.py` & `finetuner-0.7.6/finetuner/model.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.5/finetuner/names.py` & `finetuner-0.7.6/finetuner/names.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.5/finetuner/run.py` & `finetuner-0.7.6/finetuner/run.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.5/finetuner.egg-info/PKG-INFO` & `finetuner-0.7.6/finetuner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finetuner
-Version: 0.7.5
+Version: 0.7.6
 Summary: Task-oriented finetuning for better embeddings on neural search.
 Home-page: https://github.com/jina-ai/finetuner/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/finetuner/tags
 Project-URL: Documentation, https://finetuner.jina.ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: finetuner Version: 0.7.5 Summary: Task-oriented
+Metadata-Version: 2.1 Name: finetuner Version: 0.7.6 Summary: Task-oriented
 finetuning for better embeddings on neural search. Home-page: https://
 github.com/jina-ai/finetuner/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/finetuner/tags
 Project-URL: Documentation, https://finetuner.jina.ai Project-URL: Source,
 https://github.com/jina-ai/finetuner/ Project-URL: Tracker, https://github.com/
 jina-ai/finetuner/issues Description:
```

### Comparing `finetuner-0.7.5/finetuner.egg-info/SOURCES.txt` & `finetuner-0.7.6/finetuner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.5/setup.py` & `finetuner-0.7.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,22 +23,22 @@
         license='Apache 2.0',
         download_url='https://github.com/jina-ai/finetuner/tags',
         long_description=_long_description,
         long_description_content_type='text/markdown',
         zip_safe=False,
         setup_requires=['setuptools>=18.0', 'wheel'],
         install_requires=[
-            'docarray[common]>=0.21.0',
+            'docarray[common]<0.30.0',
             'trimesh==3.16.4',
-            'finetuner-stubs==0.13.3',
+            'finetuner-stubs==0.13.4',
             'jina-hubble-sdk==0.33.1',
         ],
         extras_require={
             'full': [
-                'finetuner-commons==0.13.3',
+                'finetuner-commons==0.13.4',
             ],
             'test': [
                 'black==22.3.0',
                 'flake8==5.0.4',
                 'isort==5.10.1',
                 'pytest==7.0.0',
                 'pytest-cov==3.0.0',
```

