# Comparing `tmp/envanter-1.1.2.tar.gz` & `tmp/envanter-1.2.0.tar.gz`

## Comparing `envanter-1.1.2.tar` & `envanter-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,25 @@
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 envanter-1.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 envanter-1.1.2/.readthedocs.yaml
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 envanter-1.1.2/tests.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 envanter-1.1.2/docs/Makefile
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 envanter-1.1.2/docs/source/api-reference.rst
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 envanter-1.1.2/docs/source/conf.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 envanter-1.1.2/docs/source/index.rst
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 envanter-1.1.2/docs/source/install.rst
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 envanter-1.1.2/docs/source/usage.rst
--rw-r--r--   0        0        0     8210 2020-02-02 00:00:00.000000 envanter-1.1.2/envanter/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 envanter-1.1.2/envanter/py.typed
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 envanter-1.1.2/.gitignore
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 envanter-1.1.2/LICENSE
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 envanter-1.1.2/README.md
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 envanter-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 envanter-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 envanter-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 envanter-1.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 envanter-1.2.0/test_types.py
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 envanter-1.2.0/tests.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 envanter-1.2.0/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 envanter-1.2.0/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 envanter-1.2.0/.ruff_cache/content/1003cb5b2ae3b8ad
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 envanter-1.2.0/.ruff_cache/content/76a96c6c8f125e88
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 envanter-1.2.0/.ruff_cache/content/8aae0740d0ebbb15
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 envanter-1.2.0/.ruff_cache/content/adc658ecfffe244b
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 envanter-1.2.0/.ruff_cache/content/cde67c2b0be655db
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 envanter-1.2.0/.ruff_cache/content/d103f8aec6cee9fa
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 envanter-1.2.0/docs/Makefile
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 envanter-1.2.0/docs/source/api-reference.rst
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 envanter-1.2.0/docs/source/conf.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 envanter-1.2.0/docs/source/index.rst
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 envanter-1.2.0/docs/source/install.rst
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 envanter-1.2.0/docs/source/usage.rst
+-rw-r--r--   0        0        0     8983 2020-02-02 00:00:00.000000 envanter-1.2.0/envanter/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 envanter-1.2.0/envanter/py.typed
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 envanter-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 envanter-1.2.0/LICENSE
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 envanter-1.2.0/README.md
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 envanter-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 envanter-1.2.0/PKG-INFO
```

### Comparing `envanter-1.1.2/.pre-commit-config.yaml` & `envanter-1.2.0/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -8,16 +8,15 @@
       - id: end-of-file-fixer
 
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
         exclude: migrations
-  - repo: https://github.com/PyCQA/flake8
-    rev: 6.0.0
-    hooks:
-      - id: flake8
-        exclude: migrations
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: 'v0.0.261'
+    hooks:
+      - id: ruff
```

### Comparing `envanter-1.1.2/tests.py` & `envanter-1.2.0/tests.py`

 * *Files identical despite different names*

### Comparing `envanter-1.1.2/docs/Makefile` & `envanter-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `envanter-1.1.2/docs/source/usage.rst` & `envanter-1.2.0/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `envanter-1.1.2/envanter/__init__.py` & `envanter-1.2.0/envanter/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import decimal
 import json
 import os
-from typing import Any, Callable, List, TypeVar, cast
+from typing import Any, Callable, List, TypeVar, cast, overload
 
-__version__ = "1.1.2"
+__version__ = "1.2.0"
 __all__ = ["env", "EnvironmentParser"]
 
 
 class _Empty:
     def __repr__(self) -> str:
         return "empty"
 
@@ -27,15 +27,16 @@
     """
 
     def parse(
         self,
         name: _str_T,
         /,
         default: _V = _empty,
-        parser: Callable[..., _T] = _str_F,
+        *,
+        parser: Callable[..., _T],
     ) -> _T | _V:
         """
         Allows fetching values from environment with custom parser
         function to modify it before returning.
 
         :param name: Name of the environment variable.
         :param default: Optional default value in case the variable is
@@ -50,14 +51,32 @@
             value = os.environ[name]
         except KeyError:
             if default is _empty:
                 raise
             return default
         return parser(value)
 
+    @overload
+    def list(
+        self, name: _str_T, /, default: _V = _empty, *, delimiter: _str_T = ","
+    ) -> List[str] | _V:
+        ...
+
+    @overload
+    def list(
+        self,
+        name: _str_T,
+        /,
+        default: _V = _empty,
+        *,
+        delimiter: _str_T = ",",
+        parser: Callable[..., _T],
+    ) -> List[_T] | _V:
+        ...
+
     def list(
         self,
         name: _str_T,
         /,
         default: _V = _empty,
         *,
         delimiter: _str_T = ",",
@@ -83,23 +102,46 @@
             value = os.environ[name]
         except KeyError:
             if default is _empty:
                 raise
             return default
         return [parser(item) for item in value.split(delimiter)]
 
+    @overload
     def choice(
         self,
         name: _str_T,
         /,
         default: _V = _empty,
         *,
         choices: List[_str_T],
-        parser: Callable[..., _T] = _str_F,
+    ) -> _str_T | _V:
+        ...
+
+    @overload
+    def choice(
+        self,
+        name: _str_T,
+        /,
+        default: _V = _empty,
+        *,
+        choices: List[_str_T],
+        parser: Callable[..., _T],
     ) -> _T | _V:
+        ...
+
+    def choice(
+        self,
+        name: _str_T,
+        /,
+        default: _V = _empty,
+        *,
+        choices: List[_str_T],
+        parser: Callable[..., _T] = _str_F,
+    ) -> _str_T | _T | _V:
         """
         Get an environment variable, provided that it complies with the
         choices in the related parameter. Otherwise, throws an exception
         (ValueError), with available choices.
 
         :param name: Name of the environment variable.
         :param default: Optional default value in case the variable is
@@ -217,17 +259,15 @@
         try:
             return float(os.environ[name])
         except KeyError:
             if default is _empty:
                 raise
             return default
 
-    def decimal(
-        self, name: _str_T, /, default: _T = _empty
-    ) -> decimal.Decimal | _T:
+    def decimal(self, name: _str_T, /, default: _T = _empty) -> decimal.Decimal | _T:
         """
         Get a decimal (decimal.Decimal) from environment.
 
         :param name: Name of the environment variable.
         :param default: Optional default value in case the variable is
          not found.
         :raises: ``KeyError``
```

### Comparing `envanter-1.1.2/LICENSE` & `envanter-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `envanter-1.1.2/pyproject.toml` & `envanter-1.2.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "envanter"
-version = "1.1.2"
+version = "1.2.0"
 description = "Yet another environment parser."
 readme = "README.md"
 authors = [{ name = "suayip uzulmez", email = "suayip.541@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
@@ -18,14 +18,33 @@
 requires-python = ">=3.10"
 
 [project.urls]
 "Homepage" = "https://github.com/realsuayip/envanter"
 "Bug Tracker" = "https://github.com/realsuayip/envanter/issues"
 
 [tool.black]
-line-length = 79
+line-length = 88
 
 [tool.isort]
 profile = "black"
 sections = "FUTURE,STDLIB,THIRDPARTY,FIRSTPARTY,LOCALFOLDER"
-combine_as_imports=true
-line_length = 79
+combine_as_imports = true
+line_length = 88
+
+[tool.ruff]
+select = [
+    "E", # pycodestyle errors
+    "W", # pycodestyle warnings
+    "F", # pyflakes
+    "C", # flake8-comprehensions
+    "B", # flake8-bugbear
+    "RUF", # Ruff-specific
+    "C4", # flake8-comprehensions
+    "C90", # mccabe
+]
+line-length = 88
+
+[tool.ruff.mccabe]
+max-complexity = 10
+
+[tool.mypy]
+strict = true
```

### Comparing `envanter-1.1.2/PKG-INFO` & `envanter-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: envanter
-Version: 1.1.2
+Version: 1.2.0
 Summary: Yet another environment parser.
 Project-URL: Homepage, https://github.com/realsuayip/envanter
 Project-URL: Bug Tracker, https://github.com/realsuayip/envanter/issues
 Author-email: suayip uzulmez <suayip.541@gmail.com>
 License: Copyright (c) 2022, Şuayip Üzülmez
         All rights reserved.
```

