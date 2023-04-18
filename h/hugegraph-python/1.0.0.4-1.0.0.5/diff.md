# Comparing `tmp/hugegraph-python-1.0.0.4.tar.gz` & `tmp/hugegraph-python-1.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hugegraph-python-1.0.0.4.tar", last modified: Fri Apr 14 07:59:24 2023, max compression
+gzip compressed data, was "dist/hugegraph-python-1.0.0.5.tar", last modified: Tue Apr 18 04:57:59 2023, max compression
```

## Comparing `hugegraph-python-1.0.0.4.tar` & `hugegraph-python-1.0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-04-14 07:59:24.380616 hugegraph-python-1.0.0.4/
--rw-r--r--   0 zsm        (501) staff       (20)    11357 2023-04-13 09:41:34.000000 hugegraph-python-1.0.0.4/LICENSE
--rw-r--r--   0 zsm        (501) staff       (20)     1210 2023-04-14 07:59:24.380208 hugegraph-python-1.0.0.4/PKG-INFO
--rw-rw-r--   0 zsm        (501) staff       (20)      726 2023-04-14 07:56:21.000000 hugegraph-python-1.0.0.4/README.md
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-04-14 07:59:24.378862 hugegraph-python-1.0.0.4/hugegraph_python.egg-info/
--rw-r--r--   0 zsm        (501) staff       (20)     1210 2023-04-14 07:59:24.000000 hugegraph-python-1.0.0.4/hugegraph_python.egg-info/PKG-INFO
--rw-r--r--   0 zsm        (501) staff       (20)      199 2023-04-14 07:59:24.000000 hugegraph-python-1.0.0.4/hugegraph_python.egg-info/SOURCES.txt
--rw-r--r--   0 zsm        (501) staff       (20)        1 2023-04-14 07:59:24.000000 hugegraph-python-1.0.0.4/hugegraph_python.egg-info/dependency_links.txt
--rw-r--r--   0 zsm        (501) staff       (20)        1 2023-04-14 07:59:24.000000 hugegraph-python-1.0.0.4/hugegraph_python.egg-info/top_level.txt
--rw-r--r--   0 zsm        (501) staff       (20)       38 2023-04-14 07:59:24.380715 hugegraph-python-1.0.0.4/setup.cfg
--rw-r--r--   0 zsm        (501) staff       (20)     1516 2023-04-14 07:59:05.000000 hugegraph-python-1.0.0.4/setup.py
-drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-04-14 07:59:24.379256 hugegraph-python-1.0.0.4/test/
--rw-r--r--   0 zsm        (501) staff       (20)      613 2023-04-14 07:43:44.000000 hugegraph-python-1.0.0.4/test/test.py
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-04-18 04:57:59.532528 hugegraph-python-1.0.0.5/
+-rw-r--r--   0 zsm        (501) staff       (20)    11357 2023-04-13 09:41:34.000000 hugegraph-python-1.0.0.5/LICENSE
+-rw-r--r--   0 zsm        (501) staff       (20)     1337 2023-04-18 04:57:59.532228 hugegraph-python-1.0.0.5/PKG-INFO
+-rw-rw-r--   0 zsm        (501) staff       (20)      853 2023-04-18 04:57:38.000000 hugegraph-python-1.0.0.5/README.md
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-04-18 04:57:59.531256 hugegraph-python-1.0.0.5/hugegraph_python.egg-info/
+-rw-r--r--   0 zsm        (501) staff       (20)     1337 2023-04-18 04:57:59.000000 hugegraph-python-1.0.0.5/hugegraph_python.egg-info/PKG-INFO
+-rw-r--r--   0 zsm        (501) staff       (20)      199 2023-04-18 04:57:59.000000 hugegraph-python-1.0.0.5/hugegraph_python.egg-info/SOURCES.txt
+-rw-r--r--   0 zsm        (501) staff       (20)        1 2023-04-18 04:57:59.000000 hugegraph-python-1.0.0.5/hugegraph_python.egg-info/dependency_links.txt
+-rw-r--r--   0 zsm        (501) staff       (20)        1 2023-04-18 04:57:59.000000 hugegraph-python-1.0.0.5/hugegraph_python.egg-info/top_level.txt
+-rw-r--r--   0 zsm        (501) staff       (20)       38 2023-04-18 04:57:59.532669 hugegraph-python-1.0.0.5/setup.cfg
+-rw-r--r--   0 zsm        (501) staff       (20)     1516 2023-04-18 04:57:46.000000 hugegraph-python-1.0.0.5/setup.py
+drwxr-xr-x   0 zsm        (501) staff       (20)        0 2023-04-18 04:57:59.531598 hugegraph-python-1.0.0.5/test/
+-rw-r--r--   0 zsm        (501) staff       (20)      740 2023-04-18 04:56:40.000000 hugegraph-python-1.0.0.5/test/test.py
```

### Comparing `hugegraph-python-1.0.0.4/LICENSE` & `hugegraph-python-1.0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hugegraph-python-1.0.0.4/README.md` & `hugegraph-python-1.0.0.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -23,10 +23,21 @@
 schema = client.schema()
 schema.getVertexLabels()
 
 # graph
 g = client.graph()
 g.getVertexById("1:tom")
 g.close()
+
+# gremlin
+gremlin = client.gremlin()
+gremlin.exec("g.V().limit(10)")
 ```
 
 Any questions contact [ming@apache.org](ming@apache.org)
+
+- TODO
+    - document
+    - ut
+    - ci
+    - more api
+
```

### Comparing `hugegraph-python-1.0.0.4/setup.py` & `hugegraph-python-1.0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hugegraph-python",
-    version="1.0.0.4",
+    version="1.0.0.5",
     author="cvte-research-datamining",
     author_email="ming@apache.org",
     description="A Python SDK for Apache HugeGraph",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cvte-research-datamining/hugegraph-python",
     packages=setuptools.find_packages(),
```

