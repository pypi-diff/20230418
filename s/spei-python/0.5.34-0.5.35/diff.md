# Comparing `tmp/spei_python-0.5.34.tar.gz` & `tmp/spei_python-0.5.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spei_python-0.5.34.tar", max compression
+gzip compressed data, was "spei_python-0.5.35.tar", max compression
```

## Comparing `spei_python-0.5.34.tar` & `spei_python-0.5.35.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      999 2023-02-15 18:15:34.283809 spei_python-0.5.34/README.md
--rw-r--r--   0        0        0      858 2023-03-16 01:45:26.182389 spei_python-0.5.34/pyproject.toml
--rw-r--r--   0        0        0       49 2022-07-27 23:08:37.464131 spei_python-0.5.34/spei/__init__.py
--rw-r--r--   0        0        0     2731 2023-03-09 23:20:37.585774 spei_python-0.5.34/spei/client.py
--rw-r--r--   0        0        0       66 2023-02-28 22:07:27.969521 spei_python-0.5.34/spei/resources/__init__.py
--rw-r--r--   0        0        0     3962 2023-03-13 22:05:56.750212 spei_python-0.5.34/spei/resources/ordenes.py
--rw-r--r--   0        0        0     1703 2023-03-13 21:54:51.240999 spei_python-0.5.34/spei/types.py
--rw-r--r--   0        0        0     2289 2023-03-13 22:05:00.658624 spei_python-0.5.34/spei/utils.py
--rw-r--r--   0        0        0     1637 1970-01-01 00:00:00.000000 spei_python-0.5.34/PKG-INFO
+-rw-r--r--   0        0        0      999 2023-02-15 18:15:34.283809 spei_python-0.5.35/README.md
+-rw-r--r--   0        0        0      860 2023-04-18 21:34:28.317782 spei_python-0.5.35/pyproject.toml
+-rw-r--r--   0        0        0       49 2022-07-27 23:08:37.464131 spei_python-0.5.35/spei/__init__.py
+-rw-r--r--   0        0        0     2731 2023-03-09 23:20:37.585774 spei_python-0.5.35/spei/client.py
+-rw-r--r--   0        0        0       66 2023-02-28 22:07:27.969521 spei_python-0.5.35/spei/resources/__init__.py
+-rw-r--r--   0        0        0     3962 2023-03-13 22:05:56.750212 spei_python-0.5.35/spei/resources/ordenes.py
+-rw-r--r--   0        0        0     1703 2023-03-13 21:54:51.240999 spei_python-0.5.35/spei/types.py
+-rw-r--r--   0        0        0     2289 2023-03-13 22:05:00.658624 spei_python-0.5.35/spei/utils.py
+-rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 spei_python-0.5.35/PKG-INFO
```

### Comparing `spei_python-0.5.34/README.md` & `spei_python-0.5.35/README.md`

 * *Files identical despite different names*

### Comparing `spei_python-0.5.34/pyproject.toml` & `spei_python-0.5.35/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "spei-python"
-version = "0.5.34"
+version = "0.5.35"
 description = ""
 authors = ["gonz <gonzasestopal@gmail.com>"]
 readme = "README.md"
 packages = [{include = "spei"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 lxml = "^4.9.1"
-pydantic = "1.8.2"
+pydantic = "^1.10.7"
 requests = "^2.27.1"
 cryptography = "==3.4.7"
 
 [tool.poetry.dev-dependencies]
 add-trailing-comma = "^2.2.3"
 commitizen = "^2.27.1"
 expects = "^0.9.0"
@@ -27,14 +27,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.5.34"
+version = "0.5.35"
 tag_format = "v$version"
 bump_message = "bump: Semantic Release Bot: Release Version: $new_version 🤖🚀 [skip ci]"
 version_files = [
     "pyproject.toml:version",
 ]
```

### Comparing `spei_python-0.5.34/spei/client.py` & `spei_python-0.5.35/spei/client.py`

 * *Files identical despite different names*

### Comparing `spei_python-0.5.34/spei/resources/ordenes.py` & `spei_python-0.5.35/spei/resources/ordenes.py`

 * *Files identical despite different names*

### Comparing `spei_python-0.5.34/spei/types.py` & `spei_python-0.5.35/spei/types.py`

 * *Files identical despite different names*

### Comparing `spei_python-0.5.34/spei/utils.py` & `spei_python-0.5.35/spei/utils.py`

 * *Files identical despite different names*

### Comparing `spei_python-0.5.34/PKG-INFO` & `spei_python-0.5.35/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: spei-python
-Version: 0.5.34
+Version: 0.5.35
 Summary: 
 Author: gonz
 Author-email: gonzasestopal@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cryptography (==3.4.7)
 Requires-Dist: lxml (>=4.9.1,<5.0.0)
-Requires-Dist: pydantic (==1.8.2)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 [![wemake-python-styleguide](https://img.shields.io/badge/style-wemake-000000.svg)](https://github.com/wemake-services/wemake-python-styleguide)
 
 spei-python
 ===========
```

