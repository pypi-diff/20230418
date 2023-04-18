# Comparing `tmp/plugwise_usb-0.31.0a3.tar.gz` & `tmp/plugwise_usb-0.31.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugwise_usb-0.31.0a3.tar", last modified: Tue Apr 18 19:34:45 2023, max compression
+gzip compressed data, was "plugwise_usb-0.31.0a4.tar", last modified: Tue Apr 18 19:48:52 2023, max compression
```

## Comparing `plugwise_usb-0.31.0a3.tar` & `plugwise_usb-0.31.0a4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:34:45.821727 plugwise_usb-0.31.0a3/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-18 19:34:42.000000 plugwise_usb-0.31.0a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-04-18 19:34:45.821727 plugwise_usb-0.31.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-04-18 19:34:42.000000 plugwise_usb-0.31.0a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:34:45.821727 plugwise_usb-0.31.0a3/plugwise_usb/
--rw-r--r--   0 runner    (1001) docker     (123)    30312 2023-04-18 19:34:42.000000 plugwise_usb-0.31.0a3/plugwise_usb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:34:45.821727 plugwise_usb-0.31.0a3/plugwise_usb/connections/
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-04-18 19:34:42.000000 plugwise_usb-0.31.0a3/plugwise_usb/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-18 19:34:42.000000 plugwise_usb-0.31.0a3/plugwise_usb/connections/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-18 19:34:42.000000 plugwise_usb-0.31.0a3/plugwise_usb/connections/socket.py
--rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-04-18 19:34:42.000000 plugwise_usb-0.31.0a3/plugwise_usb/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    18427 2023-04-18 19:34:42.000000 plugwise_usb-0.31.0a3/plugwise_usb/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-18 19:34:42.000000 plugwise_usb-0.31.0a3/plugwise_usb/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:34:45.821727 plugwise_usb-0.31.0a3/plugwise_usb/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-18 19:34:42.000000 plugwise_usb-0.31.0a3/plugwise_usb/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-04-18 19:34:42.000000 plugwise_usb-0.31.0a3/plugwise_usb/messages/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)    15870 2023-04-18 19:34:42.000000 plugwise_usb-0.31.0a3/plugwise_usb/messages/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:34:45.821727 plugwise_usb-0.31.0a3/plugwise_usb/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-04-18 19:34:42.000000 plugwise_usb-0.31.0a3/plugwise_usb/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35898 2023-04-18 19:34:42.000000 plugwise_usb-0.31.0a3/plugwise_usb/nodes/circle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-04-18 19:34:42.000000 plugwise_usb-0.31.0a3/plugwise_usb/nodes/circle_plus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-18 19:34:42.000000 plugwise_usb-0.31.0a3/plugwise_usb/nodes/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-04-18 19:34:42.000000 plugwise_usb-0.31.0a3/plugwise_usb/nodes/sed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-18 19:34:42.000000 plugwise_usb-0.31.0a3/plugwise_usb/nodes/sense.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-18 19:34:42.000000 plugwise_usb-0.31.0a3/plugwise_usb/nodes/stealth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-18 19:34:42.000000 plugwise_usb-0.31.0a3/plugwise_usb/nodes/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-18 19:34:42.000000 plugwise_usb-0.31.0a3/plugwise_usb/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-04-18 19:34:42.000000 plugwise_usb-0.31.0a3/plugwise_usb/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:34:45.821727 plugwise_usb-0.31.0a3/plugwise_usb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-04-18 19:34:45.000000 plugwise_usb-0.31.0a3/plugwise_usb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-18 19:34:45.000000 plugwise_usb-0.31.0a3/plugwise_usb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 19:34:45.000000 plugwise_usb-0.31.0a3/plugwise_usb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-18 19:34:45.000000 plugwise_usb-0.31.0a3/plugwise_usb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 19:34:45.000000 plugwise_usb-0.31.0a3/plugwise_usb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-04-18 19:34:42.000000 plugwise_usb-0.31.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-18 19:34:45.821727 plugwise_usb-0.31.0a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-18 19:34:42.000000 plugwise_usb-0.31.0a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:48:52.118170 plugwise_usb-0.31.0a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-18 19:48:50.000000 plugwise_usb-0.31.0a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-04-18 19:48:52.118170 plugwise_usb-0.31.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-04-18 19:48:50.000000 plugwise_usb-0.31.0a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:48:52.114170 plugwise_usb-0.31.0a4/plugwise_usb/
+-rw-r--r--   0 runner    (1001) docker     (123)    30312 2023-04-18 19:48:50.000000 plugwise_usb-0.31.0a4/plugwise_usb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:48:52.114170 plugwise_usb-0.31.0a4/plugwise_usb/connections/
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-04-18 19:48:50.000000 plugwise_usb-0.31.0a4/plugwise_usb/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-18 19:48:50.000000 plugwise_usb-0.31.0a4/plugwise_usb/connections/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-18 19:48:50.000000 plugwise_usb-0.31.0a4/plugwise_usb/connections/socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-04-18 19:48:50.000000 plugwise_usb-0.31.0a4/plugwise_usb/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18427 2023-04-18 19:48:50.000000 plugwise_usb-0.31.0a4/plugwise_usb/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-18 19:48:50.000000 plugwise_usb-0.31.0a4/plugwise_usb/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:48:52.114170 plugwise_usb-0.31.0a4/plugwise_usb/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-18 19:48:50.000000 plugwise_usb-0.31.0a4/plugwise_usb/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-04-18 19:48:50.000000 plugwise_usb-0.31.0a4/plugwise_usb/messages/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15870 2023-04-18 19:48:50.000000 plugwise_usb-0.31.0a4/plugwise_usb/messages/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:48:52.118170 plugwise_usb-0.31.0a4/plugwise_usb/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-04-18 19:48:50.000000 plugwise_usb-0.31.0a4/plugwise_usb/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35898 2023-04-18 19:48:50.000000 plugwise_usb-0.31.0a4/plugwise_usb/nodes/circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-04-18 19:48:50.000000 plugwise_usb-0.31.0a4/plugwise_usb/nodes/circle_plus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-18 19:48:50.000000 plugwise_usb-0.31.0a4/plugwise_usb/nodes/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-04-18 19:48:50.000000 plugwise_usb-0.31.0a4/plugwise_usb/nodes/sed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-18 19:48:50.000000 plugwise_usb-0.31.0a4/plugwise_usb/nodes/sense.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-18 19:48:50.000000 plugwise_usb-0.31.0a4/plugwise_usb/nodes/stealth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-18 19:48:50.000000 plugwise_usb-0.31.0a4/plugwise_usb/nodes/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-18 19:48:50.000000 plugwise_usb-0.31.0a4/plugwise_usb/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-04-18 19:48:50.000000 plugwise_usb-0.31.0a4/plugwise_usb/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:48:52.114170 plugwise_usb-0.31.0a4/plugwise_usb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-04-18 19:48:52.000000 plugwise_usb-0.31.0a4/plugwise_usb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-18 19:48:52.000000 plugwise_usb-0.31.0a4/plugwise_usb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 19:48:52.000000 plugwise_usb-0.31.0a4/plugwise_usb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-18 19:48:52.000000 plugwise_usb-0.31.0a4/plugwise_usb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 19:48:52.000000 plugwise_usb-0.31.0a4/plugwise_usb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-04-18 19:48:50.000000 plugwise_usb-0.31.0a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-18 19:48:52.118170 plugwise_usb-0.31.0a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-18 19:48:50.000000 plugwise_usb-0.31.0a4/setup.py
```

### Comparing `plugwise_usb-0.31.0a3/LICENSE` & `plugwise_usb-0.31.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `plugwise_usb-0.31.0a3/PKG-INFO` & `plugwise_usb-0.31.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugwise_usb
-Version: 0.31.0a3
+Version: 0.31.0a4
 Summary: Plugwise USB (Stick) module for Python 3.
 Home-page: https://github.com/plugwise/python-plugwise-usb
 Author: Plugwise device owners
 Maintainer: bouwew, brefra, CoMPaTech
 License: MIT License
         
         Copyright (c) 2019 @laetificat, 2019-2020 @CoMPaTech & @bouwew, 2020-current @CoMPaTech, @bouwew & @brefra
```

### Comparing `plugwise_usb-0.31.0a3/README.md` & `plugwise_usb-0.31.0a4/README.md`

 * *Files identical despite different names*

### Comparing `plugwise_usb-0.31.0a3/plugwise_usb/__init__.py` & `plugwise_usb-0.31.0a4/plugwise_usb/__init__.py`

 * *Files identical despite different names*

### Comparing `plugwise_usb-0.31.0a3/plugwise_usb/connections/__init__.py` & `plugwise_usb-0.31.0a4/plugwise_usb/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `plugwise_usb-0.31.0a3/plugwise_usb/connections/serial.py` & `plugwise_usb-0.31.0a4/plugwise_usb/connections/serial.py`

 * *Files identical despite different names*

### Comparing `plugwise_usb-0.31.0a3/plugwise_usb/connections/socket.py` & `plugwise_usb-0.31.0a4/plugwise_usb/connections/socket.py`

 * *Files identical despite different names*

### Comparing `plugwise_usb-0.31.0a3/plugwise_usb/constants.py` & `plugwise_usb-0.31.0a4/plugwise_usb/constants.py`

 * *Files identical despite different names*

### Comparing `plugwise_usb-0.31.0a3/plugwise_usb/controller.py` & `plugwise_usb-0.31.0a4/plugwise_usb/controller.py`

 * *Files identical despite different names*

### Comparing `plugwise_usb-0.31.0a3/plugwise_usb/exceptions.py` & `plugwise_usb-0.31.0a4/plugwise_usb/exceptions.py`

 * *Files identical despite different names*

### Comparing `plugwise_usb-0.31.0a3/plugwise_usb/messages/__init__.py` & `plugwise_usb-0.31.0a4/plugwise_usb/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `plugwise_usb-0.31.0a3/plugwise_usb/messages/requests.py` & `plugwise_usb-0.31.0a4/plugwise_usb/messages/requests.py`

 * *Files identical despite different names*

### Comparing `plugwise_usb-0.31.0a3/plugwise_usb/messages/responses.py` & `plugwise_usb-0.31.0a4/plugwise_usb/messages/responses.py`

 * *Files identical despite different names*

### Comparing `plugwise_usb-0.31.0a3/plugwise_usb/nodes/__init__.py` & `plugwise_usb-0.31.0a4/plugwise_usb/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `plugwise_usb-0.31.0a3/plugwise_usb/nodes/circle.py` & `plugwise_usb-0.31.0a4/plugwise_usb/nodes/circle.py`

 * *Files identical despite different names*

### Comparing `plugwise_usb-0.31.0a3/plugwise_usb/nodes/circle_plus.py` & `plugwise_usb-0.31.0a4/plugwise_usb/nodes/circle_plus.py`

 * *Files identical despite different names*

### Comparing `plugwise_usb-0.31.0a3/plugwise_usb/nodes/scan.py` & `plugwise_usb-0.31.0a4/plugwise_usb/nodes/scan.py`

 * *Files identical despite different names*

### Comparing `plugwise_usb-0.31.0a3/plugwise_usb/nodes/sed.py` & `plugwise_usb-0.31.0a4/plugwise_usb/nodes/sed.py`

 * *Files identical despite different names*

### Comparing `plugwise_usb-0.31.0a3/plugwise_usb/nodes/sense.py` & `plugwise_usb-0.31.0a4/plugwise_usb/nodes/sense.py`

 * *Files identical despite different names*

### Comparing `plugwise_usb-0.31.0a3/plugwise_usb/nodes/switch.py` & `plugwise_usb-0.31.0a4/plugwise_usb/nodes/switch.py`

 * *Files identical despite different names*

### Comparing `plugwise_usb-0.31.0a3/plugwise_usb/parser.py` & `plugwise_usb-0.31.0a4/plugwise_usb/parser.py`

 * *Files identical despite different names*

### Comparing `plugwise_usb-0.31.0a3/plugwise_usb/util.py` & `plugwise_usb-0.31.0a4/plugwise_usb/util.py`

 * *Files identical despite different names*

### Comparing `plugwise_usb-0.31.0a3/plugwise_usb.egg-info/PKG-INFO` & `plugwise_usb-0.31.0a4/plugwise_usb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugwise-usb
-Version: 0.31.0a3
+Version: 0.31.0a4
 Summary: Plugwise USB (Stick) module for Python 3.
 Home-page: https://github.com/plugwise/python-plugwise-usb
 Author: Plugwise device owners
 Maintainer: bouwew, brefra, CoMPaTech
 License: MIT License
         
         Copyright (c) 2019 @laetificat, 2019-2020 @CoMPaTech & @bouwew, 2020-current @CoMPaTech, @bouwew & @brefra
```

### Comparing `plugwise_usb-0.31.0a3/plugwise_usb.egg-info/SOURCES.txt` & `plugwise_usb-0.31.0a4/plugwise_usb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plugwise_usb-0.31.0a3/pyproject.toml` & `plugwise_usb-0.31.0a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name            = "plugwise_usb"
-version         = "0.31.0a3"
+version         = "0.31.0a4"
 license         = {file = "LICENSE"}
 description     = "Plugwise USB (Stick) module for Python 3."
 readme          = "README.md"
 keywords        = ["home", "automation", "plugwise", "module", "usb"]
 classifiers     = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

