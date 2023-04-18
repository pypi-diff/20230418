# Comparing `tmp/pyella-1.1.2.tar.gz` & `tmp/pyella-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyella-1.1.2.tar", max compression
+gzip compressed data, was "pyella-1.2.0.tar", max compression
```

## Comparing `pyella-1.1.2.tar` & `pyella-1.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    16725 2023-02-10 19:48:07.538765 pyella-1.1.2/LICENSE
--rw-r--r--   0        0        0     1847 2023-02-10 19:48:07.538765 pyella-1.1.2/README.md
--rw-r--r--   0        0        0     2612 2023-02-10 19:48:58.998492 pyella-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      159 2023-02-10 19:48:07.542765 pyella-1.1.2/src/pyella/__init__.py
--rw-r--r--   0        0        0     4506 2023-02-10 19:48:07.542765 pyella-1.1.2/src/pyella/either.py
--rw-r--r--   0        0        0     2502 2023-02-10 19:48:07.542765 pyella-1.1.2/src/pyella/maybe.py
--rw-r--r--   0        0        0     2606 1970-01-01 00:00:00.000000 pyella-1.1.2/setup.py
--rw-r--r--   0        0        0     3029 1970-01-01 00:00:00.000000 pyella-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-04-18 17:29:28.482503 pyella-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1847 2023-04-18 17:29:28.482503 pyella-1.2.0/README.md
+-rw-r--r--   0        0        0     2530 2023-04-18 17:29:57.291034 pyella-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      159 2023-04-18 17:29:28.482503 pyella-1.2.0/src/pyella/__init__.py
+-rw-r--r--   0        0        0     4715 2023-04-18 17:29:28.482503 pyella-1.2.0/src/pyella/either.py
+-rw-r--r--   0        0        0     2781 2023-04-18 17:29:28.482503 pyella-1.2.0/src/pyella/maybe.py
+-rw-r--r--   0        0        0      142 2023-04-18 17:29:28.482503 pyella-1.2.0/src/pyella/shared.py
+-rw-r--r--   0        0        0     3249 1970-01-01 00:00:00.000000 pyella-1.2.0/PKG-INFO
```

### Comparing `pyella-1.1.2/LICENSE` & `pyella-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyella-1.1.2/README.md` & `pyella-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyella-1.1.2/pyproject.toml` & `pyella-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -22,22 +22,19 @@
 keywords = [
 ]
 license = "MPL-2.0"
 maintainers = ["Ely Deckers"]
 name = "pyella"
 readme = "README.md"
 repository = "https://github.com/edeckers/pyella.git"
-version = "1.1.2"
+version = "1.2.0"
 
-[tool.poetry.dependencies]
-python = ">=3.7,<4.0"
-
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
 bandit = "^1.7"
-black = {version = "^22.6.0", allow-prereleases = true}
 coverage = {extras = ["toml"], version = "^6.3.2"}
 isort = "^5.10.1"
 mypy = "^0.931"
 nox = "^2022.1.7"
 pre-commit = "^2.17"
 pre-commit-hooks = "^4.1"
 pytest = "^7"
@@ -52,15 +49,15 @@
 log_cli = true
 log_cli_level = "INFO"
 log_cli_format = "%(asctime)s [%(levelname)8s] %(name)s: %(message)s (%(filename)s:%(lineno)s)"
 log_cli_date_format = "%Y-%m-%d %H:%M:%S"
 
 [tool.coverage.report]
 show_missing = true
-fail_under = 90
+fail_under = 94
 
 [tool.coverage.html]
 directory = "reports/coverage/html"
 
 [tool.coverage.xml]
 output = "reports/coverage/coverage.xml"
```

### Comparing `pyella-1.1.2/src/pyella/either.py` & `pyella-1.2.0/src/pyella/either.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from __future__ import annotations
 
 from argparse import ArgumentTypeError
 from typing import Callable, Generic, Iterable, List, Optional, TypeVar, Union, cast
 
 from pyella.maybe import Maybe, nothing
+from pyella.shared import _const
 
 TA = TypeVar("TA")
 TB = TypeVar("TB")
 TC = TypeVar("TC")
 TD = TypeVar("TD")
 
 
@@ -35,14 +36,17 @@
 
     def fmap(self, map_: Callable[[TB], TC]) -> Either[TA, TC]:
         return fmap(self, map_)
 
     def map_left(self, map_: Callable[[TA], TC]) -> Either[TC, TB]:
         return map_left(self, map_)
 
+    def replace(self, value: TC) -> Either[TA, TC]:
+        return replace(self, value)
+
     def if_left(self, fallback: TB) -> TB:
         return fallback if self.is_left() else cast(TB, self.value)
 
     def if_right(self, fallback: TA) -> TA:
         return fallback if self.is_right() else cast(TA, self.value)
 
     def is_left(self) -> bool:
@@ -133,14 +137,18 @@
     return Left(value)
 
 
 def lefts(eithers: Iterable[Either[TA, TB]]) -> List[TA]:
     return list(map(lambda either: cast(TA, either.value), filter(is_left, eithers)))
 
 
+def replace(self, value: TC) -> Either[TA, TC]:
+    return fmap(self, _const(value))
+
+
 def rights(eithers: Iterable[Either[TA, TB]]) -> List[TB]:
     return list(map(lambda either: cast(TB, either.value), filter(is_right, eithers)))
 
 
 def right(value: TB) -> Either[TA, TB]:
     return Right(value)
```

### Comparing `pyella-1.1.2/src/pyella/maybe.py` & `pyella-1.2.0/src/pyella/maybe.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 # LICENSE file in the root directory of this source tree.
 
 from __future__ import annotations
 
 from argparse import ArgumentTypeError
 from typing import Callable, Generic, TypeVar
 
+from pyella.shared import _const
+
 TA = TypeVar("TA")
 TB = TypeVar("TB")
 
 
 class Maybe(Generic[TA]):  # pylint: disable=too-few-public-methods
     value: TA
 
@@ -26,17 +28,24 @@
 
     def is_nothing(self) -> bool:
         return is_nothing(self)
 
     def maybe(self: Maybe[TA], fallback: TB, map_: Callable[[TA], TB]) -> TB:
         return maybe(fallback, map_, self)
 
+    def replace(self, value: TB) -> Maybe[TB]:
+        return replace(self, value)
+
     @staticmethod
     def of(value: TA):  # pylint: disable=invalid-name
-        return of(value)
+        return Maybe.pure(value)
+
+    @staticmethod
+    def pure(value: TA):
+        return pure(value)
 
     def __eq__(self, __o: object) -> bool:
         if not isinstance(__o, Maybe):
             return False
 
         if __o.is_nothing() or self.is_nothing():
             return __o.is_nothing() and self.is_nothing()
@@ -89,12 +98,16 @@
     return isinstance(em0, Nothing)
 
 
 def maybe(fallback: TB, map_: Callable[[TA], TB], em0: Maybe[TA]) -> TB:
     return fallback if is_nothing(em0) else map_(em0.value)
 
 
+def replace(self, value: TB) -> Maybe[TB]:
+    return fmap(self, _const(value))
+
+
 def of(value: TA):  # pylint: disable=invalid-name
     return nothing if value is None else Just(value)
 
 
 pure = of  # pylint: disable=invalid-name
```

### Comparing `pyella-1.1.2/PKG-INFO` & `pyella-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: pyella
-Version: 1.1.2
+Version: 1.2.0
 Summary: This library brings common monads such `Maybe` and `Either` to your Python projects.
 Home-page: https://github.com/edeckers/pyella.git
 License: MPL-2.0
 Author: Ely Deckers
 Maintainer: Ely Deckers
-Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
```

