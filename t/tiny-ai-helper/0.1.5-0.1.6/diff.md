# Comparing `tmp/tiny_ai_helper-0.1.5.tar.gz` & `tmp/tiny_ai_helper-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiny_ai_helper-0.1.5.tar", last modified: Sat Apr  8 14:07:54 2023, max compression
+gzip compressed data, was "tiny_ai_helper-0.1.6.tar", last modified: Tue Apr 18 08:30:33 2023, max compression
```

## Comparing `tiny_ai_helper-0.1.5.tar` & `tiny_ai_helper-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-04-08 14:07:54.216564 tiny_ai_helper-0.1.5/
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     1103 2023-03-09 17:46:27.000000 tiny_ai_helper-0.1.5/LICENSE
--rw-rw-r--   0 www-data  (1000) www-data  (1000)      784 2023-04-08 14:07:54.216564 tiny_ai_helper-0.1.5/PKG-INFO
--rw-rw-r--   0 www-data  (1000) www-data  (1000)       74 2022-09-27 15:48:25.000000 tiny_ai_helper-0.1.5/README.md
--rw-rw-r--   0 www-data  (1000) www-data  (1000)       38 2023-04-08 14:07:54.216564 tiny_ai_helper-0.1.5/setup.cfg
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     1029 2023-04-08 14:06:14.000000 tiny_ai_helper-0.1.5/setup.py
-drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-04-08 14:07:54.216564 tiny_ai_helper-0.1.5/tiny_ai_helper/
--rw-rw-r--   0 www-data  (1000) www-data  (1000)    14092 2023-04-08 13:19:55.000000 tiny_ai_helper-0.1.5/tiny_ai_helper/Model.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)    10280 2023-04-08 09:58:47.000000 tiny_ai_helper-0.1.5/tiny_ai_helper/Trainer.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)      367 2023-04-08 14:05:35.000000 tiny_ai_helper-0.1.5/tiny_ai_helper/__init__.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     6232 2023-03-23 11:28:02.000000 tiny_ai_helper-0.1.5/tiny_ai_helper/layers.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     9071 2023-03-15 18:42:46.000000 tiny_ai_helper-0.1.5/tiny_ai_helper/mp.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)    14131 2023-04-07 17:46:52.000000 tiny_ai_helper-0.1.5/tiny_ai_helper/utils.py
-drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-04-08 14:07:54.216564 tiny_ai_helper-0.1.5/tiny_ai_helper.egg-info/
--rw-rw-r--   0 www-data  (1000) www-data  (1000)      784 2023-04-08 14:07:52.000000 tiny_ai_helper-0.1.5/tiny_ai_helper.egg-info/PKG-INFO
--rw-rw-r--   0 www-data  (1000) www-data  (1000)      325 2023-04-08 14:07:52.000000 tiny_ai_helper-0.1.5/tiny_ai_helper.egg-info/SOURCES.txt
--rw-rw-r--   0 www-data  (1000) www-data  (1000)        1 2023-04-08 14:07:52.000000 tiny_ai_helper-0.1.5/tiny_ai_helper.egg-info/dependency_links.txt
--rw-rw-r--   0 www-data  (1000) www-data  (1000)       15 2023-04-08 14:07:52.000000 tiny_ai_helper-0.1.5/tiny_ai_helper.egg-info/top_level.txt
+drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-04-18 08:30:33.916846 tiny_ai_helper-0.1.6/
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)     1103 2023-03-09 17:46:27.000000 tiny_ai_helper-0.1.6/LICENSE
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)      784 2023-04-18 08:30:33.916846 tiny_ai_helper-0.1.6/PKG-INFO
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)       74 2022-09-27 15:48:25.000000 tiny_ai_helper-0.1.6/README.md
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)       38 2023-04-18 08:30:33.916846 tiny_ai_helper-0.1.6/setup.cfg
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)     1029 2023-04-18 08:29:21.000000 tiny_ai_helper-0.1.6/setup.py
+drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-04-18 08:30:33.916846 tiny_ai_helper-0.1.6/tiny_ai_helper/
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)    14092 2023-04-08 13:19:55.000000 tiny_ai_helper-0.1.6/tiny_ai_helper/Model.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)    10280 2023-04-08 09:58:47.000000 tiny_ai_helper-0.1.6/tiny_ai_helper/Trainer.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)      367 2023-04-18 08:29:27.000000 tiny_ai_helper-0.1.6/tiny_ai_helper/__init__.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)     6232 2023-03-23 11:28:02.000000 tiny_ai_helper-0.1.6/tiny_ai_helper/layers.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)     9071 2023-03-15 18:42:46.000000 tiny_ai_helper-0.1.6/tiny_ai_helper/mp.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)    14216 2023-04-17 11:26:04.000000 tiny_ai_helper-0.1.6/tiny_ai_helper/utils.py
+drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-04-18 08:30:33.916846 tiny_ai_helper-0.1.6/tiny_ai_helper.egg-info/
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)      784 2023-04-18 08:30:31.000000 tiny_ai_helper-0.1.6/tiny_ai_helper.egg-info/PKG-INFO
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)      325 2023-04-18 08:30:31.000000 tiny_ai_helper-0.1.6/tiny_ai_helper.egg-info/SOURCES.txt
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)        1 2023-04-18 08:30:31.000000 tiny_ai_helper-0.1.6/tiny_ai_helper.egg-info/dependency_links.txt
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)       15 2023-04-18 08:30:31.000000 tiny_ai_helper-0.1.6/tiny_ai_helper.egg-info/top_level.txt
```

### Comparing `tiny_ai_helper-0.1.5/LICENSE` & `tiny_ai_helper-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tiny_ai_helper-0.1.5/PKG-INFO` & `tiny_ai_helper-0.1.6/tiny_ai_helper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tiny_ai_helper
-Version: 0.1.5
+Name: tiny-ai-helper
+Version: 0.1.6
 Summary: Tiny AI Helper for PyTorch
 Home-page: https://github.com/bayrell/ai_helper
 Author: Ildar Bikmamatov
 Author-email: support@bayrell.org
 License: MIT License
 Keywords: ai helper,pytorch
 Platform: UNKNOWN
```

### Comparing `tiny_ai_helper-0.1.5/setup.py` & `tiny_ai_helper-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 from setuptools import setup, find_packages
 from os.path import abspath, dirname, join
 
 setup(
 	name="tiny_ai_helper",
-	version="0.1.5",
+	version="0.1.6",
 	description="Tiny AI Helper for PyTorch",
 	long_description=open(join(abspath(dirname(__file__)), 'README.md'), encoding='utf-8').read(),
 	long_description_content_type='text/markdown',
 	author="Ildar Bikmamatov",
 	author_email="support@bayrell.org",
 	license="MIT License",
 	url = "https://github.com/bayrell/ai_helper",
```

### Comparing `tiny_ai_helper-0.1.5/tiny_ai_helper/Model.py` & `tiny_ai_helper-0.1.6/tiny_ai_helper/Model.py`

 * *Files identical despite different names*

### Comparing `tiny_ai_helper-0.1.5/tiny_ai_helper/Trainer.py` & `tiny_ai_helper-0.1.6/tiny_ai_helper/Trainer.py`

 * *Files identical despite different names*

### Comparing `tiny_ai_helper-0.1.5/tiny_ai_helper/layers.py` & `tiny_ai_helper-0.1.6/tiny_ai_helper/layers.py`

 * *Files identical despite different names*

### Comparing `tiny_ai_helper-0.1.5/tiny_ai_helper/mp.py` & `tiny_ai_helper-0.1.6/tiny_ai_helper/mp.py`

 * *Files identical despite different names*

### Comparing `tiny_ai_helper-0.1.5/tiny_ai_helper/utils.py` & `tiny_ai_helper-0.1.6/tiny_ai_helper/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -484,14 +484,16 @@
             "params_count": 0,
             "params_train_count": 0,
             "total_size": 0,
         }
         
         def forward_hook(module, input, output):
             
+            output = output[0] if isinstance(output, tuple) else output
+            
             class_name = module.__class__.__module__ + "." + module.__class__.__name__
             layer = {
                 "name": module.__class__.__name__,
                 "class_name": module.__class__.__module__ + "." + module.__class__.__name__,
                 "shape": output.shape,
                 "params": 0
             }
```

### Comparing `tiny_ai_helper-0.1.5/tiny_ai_helper.egg-info/PKG-INFO` & `tiny_ai_helper-0.1.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tiny-ai-helper
-Version: 0.1.5
+Name: tiny_ai_helper
+Version: 0.1.6
 Summary: Tiny AI Helper for PyTorch
 Home-page: https://github.com/bayrell/ai_helper
 Author: Ildar Bikmamatov
 Author-email: support@bayrell.org
 License: MIT License
 Keywords: ai helper,pytorch
 Platform: UNKNOWN
```

