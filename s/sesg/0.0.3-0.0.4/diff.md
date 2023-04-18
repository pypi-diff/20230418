# Comparing `tmp/sesg-0.0.3.tar.gz` & `tmp/sesg-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sesg-0.0.3.tar", max compression
+gzip compressed data, was "sesg-0.0.4.tar", max compression
```

## Comparing `sesg-0.0.3.tar` & `sesg-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35148 2023-04-17 17:41:20.988197 sesg-0.0.3/LICENSE
--rw-r--r--   0        0        0      478 2023-04-17 17:33:48.160350 sesg-0.0.3/README.md
--rw-r--r--   0        0        0     3014 2023-04-18 04:45:02.663654 sesg-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       47 2023-04-17 15:18:13.051151 sesg-0.0.3/src/sesg/__init__.py
--rw-r--r--   0        0        0     8127 2023-04-17 21:13:02.702530 sesg-0.0.3/src/sesg/graph.py
--rw-r--r--   0        0        0     6744 2023-04-17 14:56:33.924330 sesg-0.0.3/src/sesg/metrics.py
--rw-r--r--   0        0        0      173 2023-04-18 04:38:35.955358 sesg-0.0.3/src/sesg/scopus/__init__.py
--rw-r--r--   0        0        0     7628 2023-04-18 04:43:47.784342 sesg-0.0.3/src/sesg/scopus/api.py
--rw-r--r--   0        0        0     5914 2023-04-18 04:39:34.710767 sesg-0.0.3/src/sesg/scopus/client.py
--rw-r--r--   0        0        0    16416 2023-04-18 03:04:34.582222 sesg-0.0.3/src/sesg/scopus_client.py
--rw-r--r--   0        0        0    13843 2023-04-18 03:31:52.519891 sesg-0.0.3/src/sesg/search_string.py
--rw-r--r--   0        0        0     7659 2023-04-17 15:00:57.692606 sesg-0.0.3/src/sesg/snowballing.py
--rw-r--r--   0        0        0     5056 2023-04-16 16:49:33.237266 sesg-0.0.3/src/sesg/topic_extraction.py
--rw-r--r--   0        0        0     1829 1970-01-01 00:00:00.000000 sesg-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-04-17 17:41:20.988197 sesg-0.0.4/LICENSE
+-rw-r--r--   0        0        0      478 2023-04-17 17:33:48.160350 sesg-0.0.4/README.md
+-rw-r--r--   0        0        0     2779 2023-04-18 04:54:00.660082 sesg-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-04-17 15:18:13.051151 sesg-0.0.4/src/sesg/__init__.py
+-rw-r--r--   0        0        0     8127 2023-04-17 21:13:02.702530 sesg-0.0.4/src/sesg/graph.py
+-rw-r--r--   0        0        0     6744 2023-04-17 14:56:33.924330 sesg-0.0.4/src/sesg/metrics.py
+-rw-r--r--   0        0        0      173 2023-04-18 04:38:35.955358 sesg-0.0.4/src/sesg/scopus/__init__.py
+-rw-r--r--   0        0        0     7628 2023-04-18 04:43:47.784342 sesg-0.0.4/src/sesg/scopus/api.py
+-rw-r--r--   0        0        0     5914 2023-04-18 04:39:34.710767 sesg-0.0.4/src/sesg/scopus/client.py
+-rw-r--r--   0        0        0    16416 2023-04-18 03:04:34.582222 sesg-0.0.4/src/sesg/scopus_client.py
+-rw-r--r--   0        0        0    13843 2023-04-18 03:31:52.519891 sesg-0.0.4/src/sesg/search_string.py
+-rw-r--r--   0        0        0     7659 2023-04-17 15:00:57.692606 sesg-0.0.4/src/sesg/snowballing.py
+-rw-r--r--   0        0        0     5056 2023-04-16 16:49:33.237266 sesg-0.0.4/src/sesg/topic_extraction.py
+-rw-r--r--   0        0        0     1829 1970-01-01 00:00:00.000000 sesg-0.0.4/PKG-INFO
```

### Comparing `sesg-0.0.3/LICENSE` & `sesg-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sesg-0.0.3/pyproject.toml` & `sesg-0.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sesg"
-version = "0.0.3"
+version = "0.0.4"
 description = "SeSG is a tool developed to help Systematic Literature Review researchers, specifically at the step of building a search string."
 authors = ["Demetrius Panovitch <demetrius.mp789@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [
   {include = "sesg", from = "src"}
 ]
@@ -51,25 +51,14 @@
 mkdocs-literate-nav = "^0.6.0"
 mkdocs-section-index = "^0.3.5"
 
 
 [tool.poetry.group.dev.dependencies]
 taskipy = "^1.10.4"
 
-
-[tool.poetry.group.experiment.dependencies]
-sqlalchemy = "^2.0.9"
-typer = {extras = ["all"], version = "^0.7.0"}
-python-dotenv = "^1.0.0"
-dacite = "^1.8.0"
-tomli = "^2.0.1"
-rich = "12.6.0"
-tomli-w = "^1.0.0"
-transformers = "^4.28.1"
-
 [tool.ruff]
 extend-select = ["I001"]
 unfixable = ["F841"]
 exclude = [".venv"]
 
 [tool.ruff.pydocstyle]
 convention = "google"
```

### Comparing `sesg-0.0.3/src/sesg/graph.py` & `sesg-0.0.4/src/sesg/graph.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.3/src/sesg/metrics.py` & `sesg-0.0.4/src/sesg/metrics.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.3/src/sesg/scopus/api.py` & `sesg-0.0.4/src/sesg/scopus/api.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.3/src/sesg/scopus/client.py` & `sesg-0.0.4/src/sesg/scopus/client.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.3/src/sesg/scopus_client.py` & `sesg-0.0.4/src/sesg/scopus_client.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.3/src/sesg/search_string.py` & `sesg-0.0.4/src/sesg/search_string.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.3/src/sesg/snowballing.py` & `sesg-0.0.4/src/sesg/snowballing.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.3/src/sesg/topic_extraction.py` & `sesg-0.0.4/src/sesg/topic_extraction.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.3/PKG-INFO` & `sesg-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sesg
-Version: 0.0.3
+Version: 0.0.4
 Summary: SeSG is a tool developed to help Systematic Literature Review researchers, specifically at the step of building a search string.
 License: GPL-3.0-only
 Author: Demetrius Panovitch
 Author-email: demetrius.mp789@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

