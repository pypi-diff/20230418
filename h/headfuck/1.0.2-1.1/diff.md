# Comparing `tmp/headfuck-1.0.2.tar.gz` & `tmp/headfuck-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "headfuck-1.0.2.tar", max compression
+gzip compressed data, was "headfuck-1.1.tar", max compression
```

## Comparing `headfuck-1.0.2.tar` & `headfuck-1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1211 2023-04-17 22:22:36.300042 headfuck-1.0.2/LICENSE
--rw-r--r--   0        0        0     1094 2023-04-17 22:46:53.278302 headfuck-1.0.2/README.md
--rw-r--r--   0        0        0        0 2023-04-17 22:03:23.039464 headfuck-1.0.2/headfuck/__init__.py
--rw-r--r--   0        0        0       19 2023-04-17 22:38:15.468576 headfuck-1.0.2/headfuck/file.bf
--rw-r--r--   0        0        0      369 2023-04-17 22:43:35.306725 headfuck-1.0.2/headfuck/hff.py
--rw-r--r--   0        0        0     3405 2023-04-17 22:46:11.747278 headfuck-1.0.2/headfuck/interpreter.py
--rw-r--r--   0        0        0      590 2023-04-17 22:55:17.950576 headfuck-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1620 1970-01-01 00:00:00.000000 headfuck-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-17 22:22:36.300042 headfuck-1.1/LICENSE
+-rw-r--r--   0        0        0     1094 2023-04-17 22:46:53.278302 headfuck-1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 22:03:23.039464 headfuck-1.1/headfuck/__init__.py
+-rw-r--r--   0        0        0       19 2023-04-17 22:38:15.468576 headfuck-1.1/headfuck/file.bf
+-rw-r--r--   0        0        0      369 2023-04-17 22:43:35.306725 headfuck-1.1/headfuck/hff.py
+-rw-r--r--   0        0        0     3405 2023-04-17 22:46:11.747278 headfuck-1.1/headfuck/interpreter.py
+-rw-r--r--   0        0        0      588 2023-04-17 22:56:18.942045 headfuck-1.1/pyproject.toml
+-rw-r--r--   0        0        0     1618 1970-01-01 00:00:00.000000 headfuck-1.1/PKG-INFO
```

### Comparing `headfuck-1.0.2/LICENSE` & `headfuck-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `headfuck-1.0.2/README.md` & `headfuck-1.1/README.md`

 * *Files identical despite different names*

### Comparing `headfuck-1.0.2/headfuck/interpreter.py` & `headfuck-1.1/headfuck/interpreter.py`

 * *Files identical despite different names*

### Comparing `headfuck-1.0.2/pyproject.toml` & `headfuck-1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "headfuck"
-version = "1.0.2"
+version = "1.1"
 description = "An esoteric programming language similar to Brainfuck"
 authors = ["JJPMaster <joshuaponce2008@gmail.com>"]
 readme = "README.md"
 packages = [{include = "headfuck"}]
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: Public Domain",
```

### Comparing `headfuck-1.0.2/PKG-INFO` & `headfuck-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: headfuck
-Version: 1.0.2
+Version: 1.1
 Summary: An esoteric programming language similar to Brainfuck
 Author: JJPMaster
 Author-email: joshuaponce2008@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

