# Comparing `tmp/protoletariat-3.2.2.tar.gz` & `tmp/protoletariat-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protoletariat-3.2.2.tar", max compression
+gzip compressed data, was "protoletariat-3.2.3.tar", max compression
```

## Comparing `protoletariat-3.2.2.tar` & `protoletariat-3.2.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-04-13 07:43:58.688636 protoletariat-3.2.2/LICENSE
--rw-r--r--   0        0        0     5066 2023-04-13 07:43:58.688636 protoletariat-3.2.2/README.md
--rw-r--r--   0        0        0       66 2023-04-13 07:45:03.600724 protoletariat-3.2.2/protoletariat/__init__.py
--rw-r--r--   0        0        0     4333 2023-04-13 07:43:58.688636 protoletariat-3.2.2/protoletariat/__main__.py
--rw-r--r--   0        0        0     6661 2023-04-13 07:43:58.688636 protoletariat-3.2.2/protoletariat/fdsetgen.py
--rw-r--r--   0        0        0     7641 2023-04-13 07:43:58.688636 protoletariat-3.2.2/protoletariat/rewrite.py
--rw-r--r--   0        0        0        0 2023-04-13 07:43:58.688636 protoletariat-3.2.2/protoletariat/tests/__init__.py
--rw-r--r--   0        0        0    24371 2023-04-13 07:43:58.688636 protoletariat-3.2.2/protoletariat/tests/conftest.py
--rw-r--r--   0        0        0     7772 2023-04-13 07:43:58.688636 protoletariat-3.2.2/protoletariat/tests/test_fix_imports.py
--rw-r--r--   0        0        0     3004 2023-04-13 07:43:58.688636 protoletariat-3.2.2/protoletariat/tests/test_rewrite.py
--rw-r--r--   0        0        0     3849 2023-04-13 07:45:06.444731 protoletariat-3.2.2/pyproject.toml
--rw-r--r--   0        0        0     6425 1970-01-01 00:00:00.000000 protoletariat-3.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-18 18:16:10.462166 protoletariat-3.2.3/LICENSE
+-rw-r--r--   0        0        0     5066 2023-04-18 18:16:10.462166 protoletariat-3.2.3/README.md
+-rw-r--r--   0        0        0       66 2023-04-18 18:17:13.197795 protoletariat-3.2.3/protoletariat/__init__.py
+-rw-r--r--   0        0        0     4333 2023-04-18 18:16:10.466166 protoletariat-3.2.3/protoletariat/__main__.py
+-rw-r--r--   0        0        0     6661 2023-04-18 18:16:10.466166 protoletariat-3.2.3/protoletariat/fdsetgen.py
+-rw-r--r--   0        0        0     7641 2023-04-18 18:16:10.466166 protoletariat-3.2.3/protoletariat/rewrite.py
+-rw-r--r--   0        0        0        0 2023-04-18 18:16:10.466166 protoletariat-3.2.3/protoletariat/tests/__init__.py
+-rw-r--r--   0        0        0    24371 2023-04-18 18:16:10.466166 protoletariat-3.2.3/protoletariat/tests/conftest.py
+-rw-r--r--   0        0        0     7772 2023-04-18 18:16:10.466166 protoletariat-3.2.3/protoletariat/tests/test_fix_imports.py
+-rw-r--r--   0        0        0     3004 2023-04-18 18:16:10.466166 protoletariat-3.2.3/protoletariat/tests/test_rewrite.py
+-rw-r--r--   0        0        0     3849 2023-04-18 18:17:16.009778 protoletariat-3.2.3/pyproject.toml
+-rw-r--r--   0        0        0     6425 1970-01-01 00:00:00.000000 protoletariat-3.2.3/PKG-INFO
```

### Comparing `protoletariat-3.2.2/LICENSE` & `protoletariat-3.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `protoletariat-3.2.2/README.md` & `protoletariat-3.2.3/README.md`

 * *Files identical despite different names*

### Comparing `protoletariat-3.2.2/protoletariat/__main__.py` & `protoletariat-3.2.3/protoletariat/__main__.py`

 * *Files identical despite different names*

### Comparing `protoletariat-3.2.2/protoletariat/fdsetgen.py` & `protoletariat-3.2.3/protoletariat/fdsetgen.py`

 * *Files identical despite different names*

### Comparing `protoletariat-3.2.2/protoletariat/rewrite.py` & `protoletariat-3.2.3/protoletariat/rewrite.py`

 * *Files identical despite different names*

### Comparing `protoletariat-3.2.2/protoletariat/tests/conftest.py` & `protoletariat-3.2.3/protoletariat/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `protoletariat-3.2.2/protoletariat/tests/test_fix_imports.py` & `protoletariat-3.2.3/protoletariat/tests/test_fix_imports.py`

 * *Files identical despite different names*

### Comparing `protoletariat-3.2.2/protoletariat/tests/test_rewrite.py` & `protoletariat-3.2.3/protoletariat/tests/test_rewrite.py`

 * *Files identical despite different names*

### Comparing `protoletariat-3.2.2/pyproject.toml` & `protoletariat-3.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "protoletariat"
-version = "3.2.2"
+version = "3.2.3"
 packages = [{ include = "protoletariat" }]
 homepage = "https://github.com/cpcloud/protoletariat"
 repository = "https://github.com/cpcloud/protoletariat"
 description = "Python protocol buffers for the rest of us"
 authors = ["Phillip Cloud <417981+cpcloud@users.noreply.github.com>"]
 maintainers = ["Phillip Cloud <417981+cpcloud@users.noreply.github.com>"]
 license = "Apache-2.0"
```

### Comparing `protoletariat-3.2.2/PKG-INFO` & `protoletariat-3.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protoletariat
-Version: 3.2.2
+Version: 3.2.3
 Summary: Python protocol buffers for the rest of us
 Home-page: https://github.com/cpcloud/protoletariat
 License: Apache-2.0
 Author: Phillip Cloud
 Author-email: 417981+cpcloud@users.noreply.github.com
 Maintainer: Phillip Cloud
 Maintainer-email: 417981+cpcloud@users.noreply.github.com
```

