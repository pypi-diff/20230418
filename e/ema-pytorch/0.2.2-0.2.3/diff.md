# Comparing `tmp/ema-pytorch-0.2.2.tar.gz` & `tmp/ema-pytorch-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ema-pytorch-0.2.2.tar", last modified: Thu Mar 23 18:02:11 2023, max compression
+gzip compressed data, was "ema-pytorch-0.2.3.tar", last modified: Tue Apr 18 03:25:59 2023, max compression
```

## Comparing `ema-pytorch-0.2.2.tar` & `ema-pytorch-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:02:11.093633 ema-pytorch-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-23 18:01:59.000000 ema-pytorch-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-23 18:02:11.093633 ema-pytorch-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-03-23 18:01:59.000000 ema-pytorch-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:02:11.093633 ema-pytorch-0.2.2/ema_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-23 18:01:59.000000 ema-pytorch-0.2.2/ema_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-03-23 18:01:59.000000 ema-pytorch-0.2.2/ema_pytorch/ema_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:02:11.093633 ema-pytorch-0.2.2/ema_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-23 18:02:11.000000 ema-pytorch-0.2.2/ema_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-23 18:02:11.000000 ema-pytorch-0.2.2/ema_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 18:02:11.000000 ema-pytorch-0.2.2/ema_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-23 18:02:11.000000 ema-pytorch-0.2.2/ema_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-23 18:02:11.000000 ema-pytorch-0.2.2/ema_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 18:02:11.093633 ema-pytorch-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-23 18:01:59.000000 ema-pytorch-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:25:59.498843 ema-pytorch-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-18 03:25:46.000000 ema-pytorch-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-18 03:25:59.498843 ema-pytorch-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-18 03:25:46.000000 ema-pytorch-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:25:59.494843 ema-pytorch-0.2.3/ema_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 03:25:46.000000 ema-pytorch-0.2.3/ema_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-04-18 03:25:46.000000 ema-pytorch-0.2.3/ema_pytorch/ema_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 03:25:59.498843 ema-pytorch-0.2.3/ema_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-18 03:25:59.000000 ema-pytorch-0.2.3/ema_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-18 03:25:59.000000 ema-pytorch-0.2.3/ema_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 03:25:59.000000 ema-pytorch-0.2.3/ema_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 03:25:59.000000 ema-pytorch-0.2.3/ema_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 03:25:59.000000 ema-pytorch-0.2.3/ema_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 03:25:59.498843 ema-pytorch-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-18 03:25:46.000000 ema-pytorch-0.2.3/setup.py
```

### Comparing `ema-pytorch-0.2.2/LICENSE` & `ema-pytorch-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ema-pytorch-0.2.2/PKG-INFO` & `ema-pytorch-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ema-pytorch
-Version: 0.2.2
+Version: 0.2.3
 Summary: Easy way to keep track of exponential moving average version of your pytorch module
 Home-page: https://github.com/lucidrains/ema-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,exponential moving average
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ema-pytorch-0.2.2/README.md` & `ema-pytorch-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ema-pytorch-0.2.2/ema_pytorch/ema_pytorch.py` & `ema-pytorch-0.2.3/ema_pytorch/ema_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,16 +71,16 @@
                 self.ema_model = copy.deepcopy(model)
             except:
                 print('Your model was not copyable. Please make sure you are not using any LazyLinear')
                 exit()
 
         self.ema_model.requires_grad_(False)
 
-        self.parameter_names = {name for name, param in self.ema_model.named_parameters() if param.dtype == torch.float}
-        self.buffer_names = {name for name, buffer in self.ema_model.named_buffers() if buffer.dtype == torch.float}
+        self.parameter_names = {name for name, param in self.ema_model.named_parameters() if param.dtype in [torch.float, torch.float16]}
+        self.buffer_names = {name for name, buffer in self.ema_model.named_buffers() if buffer.dtype in [torch.float, torch.float16]}
 
         self.update_every = update_every
         self.update_after_step = update_after_step
 
         self.inv_gamma = inv_gamma
         self.power = power
         self.min_value = min_value
```

### Comparing `ema-pytorch-0.2.2/ema_pytorch.egg-info/PKG-INFO` & `ema-pytorch-0.2.3/ema_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ema-pytorch
-Version: 0.2.2
+Version: 0.2.3
 Summary: Easy way to keep track of exponential moving average version of your pytorch module
 Home-page: https://github.com/lucidrains/ema-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,exponential moving average
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ema-pytorch-0.2.2/setup.py` & `ema-pytorch-0.2.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'ema-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.2.2',
+  version = '0.2.3',
   license='MIT',
   description = 'Easy way to keep track of exponential moving average version of your pytorch module',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/ema-pytorch',
   keywords = [
```

