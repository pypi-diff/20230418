# Comparing `tmp/nua_lib-0.5.11.tar.gz` & `tmp/nua_lib-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nua_lib-0.5.11.tar", max compression
+gzip compressed data, was "nua_lib-0.5.9.tar", max compression
```

## Comparing `nua_lib-0.5.11.tar` & `nua_lib-0.5.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      544 2023-02-06 17:21:30.498783 nua_lib-0.5.11/README.md
--rw-r--r--   0        0        0     1241 2023-04-18 16:54:53.286030 nua_lib-0.5.11/pyproject.toml
--rw-r--r--   0        0        0      218 2023-02-06 17:21:30.499791 nua_lib-0.5.11/src/nua/lib/__init__.py
--rw-r--r--   0        0        0    21348 2023-04-18 14:45:14.195218 nua_lib-0.5.11/src/nua/lib/actions.py
--rw-r--r--   0        0        0      769 2023-01-11 17:39:15.272394 nua_lib-0.5.11/src/nua/lib/backports.py
--rw-r--r--   0        0        0     1344 2023-04-18 14:45:14.195754 nua_lib-0.5.11/src/nua/lib/console.py
--rw-r--r--   0        0        0     5600 2023-03-06 16:13:43.253043 nua_lib-0.5.11/src/nua/lib/exec.py
--rw-r--r--   0        0        0      828 2023-04-08 16:30:34.876808 nua_lib-0.5.11/src/nua/lib/gen_password.py
--rw-r--r--   0        0        0     1948 2023-04-18 14:45:14.196144 nua_lib-0.5.11/src/nua/lib/panic.py
--rw-r--r--   0        0        0     3932 2023-04-08 16:18:44.073176 nua_lib-0.5.11/src/nua/lib/shell.py
--rw-r--r--   0        0        0       60 2023-02-06 17:21:30.499928 nua_lib-0.5.11/src/nua/lib/tool/__init__.py
--rw-r--r--   0        0        0     3509 2023-04-08 16:30:35.028834 nua_lib-0.5.11/src/nua/lib/tool/color_str.py
--rw-r--r--   0        0        0     1133 2023-02-13 14:04:49.214475 nua_lib-0.5.11/src/nua/lib/tool/state.py
--rw-r--r--   0        0        0     2077 2023-03-21 16:25:52.745820 nua_lib-0.5.11/src/nua/lib/unarchiver.py
--rw-r--r--   0        0        0       79 2023-01-03 14:14:59.347734 nua_lib-0.5.11/src/nua/lib/version.py
--rw-r--r--   0        0        0     1028 1970-01-01 00:00:00.000000 nua_lib-0.5.11/PKG-INFO
+-rw-r--r--   0        0        0      544 2023-02-06 17:21:30.498783 nua_lib-0.5.9/README.md
+-rw-r--r--   0        0        0     1240 2023-04-18 16:37:02.790822 nua_lib-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0      218 2023-02-06 17:21:30.499791 nua_lib-0.5.9/src/nua/lib/__init__.py
+-rw-r--r--   0        0        0    21348 2023-04-18 14:45:14.195218 nua_lib-0.5.9/src/nua/lib/actions.py
+-rw-r--r--   0        0        0      769 2023-01-11 17:39:15.272394 nua_lib-0.5.9/src/nua/lib/backports.py
+-rw-r--r--   0        0        0     1344 2023-04-18 14:45:14.195754 nua_lib-0.5.9/src/nua/lib/console.py
+-rw-r--r--   0        0        0     5600 2023-03-06 16:13:43.253043 nua_lib-0.5.9/src/nua/lib/exec.py
+-rw-r--r--   0        0        0      828 2023-04-08 16:30:34.876808 nua_lib-0.5.9/src/nua/lib/gen_password.py
+-rw-r--r--   0        0        0     1948 2023-04-18 14:45:14.196144 nua_lib-0.5.9/src/nua/lib/panic.py
+-rw-r--r--   0        0        0     3932 2023-04-08 16:18:44.073176 nua_lib-0.5.9/src/nua/lib/shell.py
+-rw-r--r--   0        0        0       60 2023-02-06 17:21:30.499928 nua_lib-0.5.9/src/nua/lib/tool/__init__.py
+-rw-r--r--   0        0        0     3509 2023-04-08 16:30:35.028834 nua_lib-0.5.9/src/nua/lib/tool/color_str.py
+-rw-r--r--   0        0        0     1133 2023-02-13 14:04:49.214475 nua_lib-0.5.9/src/nua/lib/tool/state.py
+-rw-r--r--   0        0        0     2077 2023-03-21 16:25:52.745820 nua_lib-0.5.9/src/nua/lib/unarchiver.py
+-rw-r--r--   0        0        0       79 2023-01-03 14:14:59.347734 nua_lib-0.5.9/src/nua/lib/version.py
+-rw-r--r--   0        0        0     1027 1970-01-01 00:00:00.000000 nua_lib-0.5.9/PKG-INFO
```

### Comparing `nua_lib-0.5.11/README.md` & `nua_lib-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `nua_lib-0.5.11/pyproject.toml` & `nua_lib-0.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nua-lib"
-version = "0.5.11"
+version = "0.5.9"
 description = "Nua common library"
 authors = ["Stefane Fermigier <sf@abilian.com>", "Jerome Dumonteil <jd@abilian.com>"]
 license = "AGPL"
 readme = "README.md"
 packages = [
   { include = "nua", from = "src" }
 ]
```

### Comparing `nua_lib-0.5.11/src/nua/lib/actions.py` & `nua_lib-0.5.9/src/nua/lib/actions.py`

 * *Files identical despite different names*

### Comparing `nua_lib-0.5.11/src/nua/lib/backports.py` & `nua_lib-0.5.9/src/nua/lib/backports.py`

 * *Files identical despite different names*

### Comparing `nua_lib-0.5.11/src/nua/lib/console.py` & `nua_lib-0.5.9/src/nua/lib/console.py`

 * *Files identical despite different names*

### Comparing `nua_lib-0.5.11/src/nua/lib/exec.py` & `nua_lib-0.5.9/src/nua/lib/exec.py`

 * *Files identical despite different names*

### Comparing `nua_lib-0.5.11/src/nua/lib/gen_password.py` & `nua_lib-0.5.9/src/nua/lib/gen_password.py`

 * *Files identical despite different names*

### Comparing `nua_lib-0.5.11/src/nua/lib/panic.py` & `nua_lib-0.5.9/src/nua/lib/panic.py`

 * *Files identical despite different names*

### Comparing `nua_lib-0.5.11/src/nua/lib/shell.py` & `nua_lib-0.5.9/src/nua/lib/shell.py`

 * *Files identical despite different names*

### Comparing `nua_lib-0.5.11/src/nua/lib/tool/color_str.py` & `nua_lib-0.5.9/src/nua/lib/tool/color_str.py`

 * *Files identical despite different names*

### Comparing `nua_lib-0.5.11/src/nua/lib/tool/state.py` & `nua_lib-0.5.9/src/nua/lib/tool/state.py`

 * *Files identical despite different names*

### Comparing `nua_lib-0.5.11/src/nua/lib/unarchiver.py` & `nua_lib-0.5.9/src/nua/lib/unarchiver.py`

 * *Files identical despite different names*

### Comparing `nua_lib-0.5.11/PKG-INFO` & `nua_lib-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nua-lib
-Version: 0.5.11
+Version: 0.5.9
 Summary: Nua common library
 License: AGPL
 Author: Stefane Fermigier
 Author-email: sf@abilian.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

