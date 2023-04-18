# Comparing `tmp/vutils-testing-0.6.2.tar.gz` & `tmp/vutils-testing-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vutils-testing-0.6.2.tar", last modified: Mon Mar  6 01:38:47 2023, max compression
+gzip compressed data, was "vutils-testing-1.0.0.tar", last modified: Tue Apr 18 19:02:12 2023, max compression
```

## Comparing `vutils-testing-0.6.2.tar` & `vutils-testing-1.0.0.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:38:47.930239 vutils-testing-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-06 01:38:31.000000 vutils-testing-0.6.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-03-06 01:38:31.000000 vutils-testing-0.6.2/ChangeLog.md
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-06 01:38:31.000000 vutils-testing-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-06 01:38:31.000000 vutils-testing-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-03-06 01:38:47.930239 vutils-testing-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-03-06 01:38:31.000000 vutils-testing-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-03-06 01:38:31.000000 vutils-testing-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-03-06 01:38:47.934239 vutils-testing-0.6.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      298 2023-03-06 01:38:31.000000 vutils-testing-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:38:47.926238 vutils-testing-0.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:38:47.926238 vutils-testing-0.6.2/src/vutils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:38:47.930239 vutils-testing-0.6.2/src/vutils/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-06 01:38:31.000000 vutils-testing-0.6.2/src/vutils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-06 01:38:31.000000 vutils-testing-0.6.2/src/vutils/testing/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-03-06 01:38:31.000000 vutils-testing-0.6.2/src/vutils/testing/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 01:38:31.000000 vutils-testing-0.6.2/src/vutils/testing/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-03-06 01:38:31.000000 vutils-testing-0.6.2/src/vutils/testing/testcase.py
--rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-03-06 01:38:31.000000 vutils-testing-0.6.2/src/vutils/testing/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-06 01:38:31.000000 vutils-testing-0.6.2/src/vutils/testing/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:38:47.930239 vutils-testing-0.6.2/src/vutils_testing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-03-06 01:38:47.000000 vutils-testing-0.6.2/src/vutils_testing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-03-06 01:38:47.000000 vutils-testing-0.6.2/src/vutils_testing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 01:38:47.000000 vutils-testing-0.6.2/src/vutils_testing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 01:38:47.000000 vutils-testing-0.6.2/src/vutils_testing.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-06 01:38:47.000000 vutils-testing-0.6.2/src/vutils_testing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-06 01:38:47.000000 vutils-testing-0.6.2/src/vutils_testing.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:38:47.926238 vutils-testing-0.6.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:38:47.930239 vutils-testing-0.6.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-03-06 01:38:31.000000 vutils-testing-0.6.2/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-03-06 01:38:31.000000 vutils-testing-0.6.2/tests/unit/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-03-06 01:38:31.000000 vutils-testing-0.6.2/tests/unit/test_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-03-06 01:38:31.000000 vutils-testing-0.6.2/tests/unit/test_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-03-06 01:38:31.000000 vutils-testing-0.6.2/tests/unit/test_testcase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-03-06 01:38:31.000000 vutils-testing-0.6.2/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-06 01:38:31.000000 vutils-testing-0.6.2/tests/unit/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-03-06 01:38:31.000000 vutils-testing-0.6.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:02:12.124873 vutils-testing-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/ChangeLog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-18 19:02:12.124873 vutils-testing-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-18 19:02:12.124873 vutils-testing-1.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      298 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:02:12.120873 vutils-testing-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:02:12.120873 vutils-testing-1.0.0/src/vutils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:02:12.120873 vutils-testing-1.0.0/src/vutils/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/src/vutils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/src/vutils/testing/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/src/vutils/testing/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/src/vutils/testing/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/src/vutils/testing/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/src/vutils/testing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/src/vutils/testing/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:02:12.124873 vutils-testing-1.0.0/src/vutils_testing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-18 19:02:12.000000 vutils-testing-1.0.0/src/vutils_testing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-18 19:02:12.000000 vutils-testing-1.0.0/src/vutils_testing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 19:02:12.000000 vutils-testing-1.0.0/src/vutils_testing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 19:02:12.000000 vutils-testing-1.0.0/src/vutils_testing.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-18 19:02:12.000000 vutils-testing-1.0.0/src/vutils_testing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 19:02:12.000000 vutils-testing-1.0.0/src/vutils_testing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:02:12.120873 vutils-testing-1.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:02:12.124873 vutils-testing-1.0.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/tests/unit/test_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/tests/unit/test_testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/tests/unit/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/tests/unit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-18 19:01:59.000000 vutils-testing-1.0.0/tox.ini
```

### Comparing `vutils-testing-0.6.2/ChangeLog.md` & `vutils-testing-1.0.0/ChangeLog.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Change Log
 
+## 1.0.0
+
+* Move the development status to production/stable
+* Code cleanup
+
 ## 0.6.2
 
 * Fix `safety` issues
 
 ## 0.6.1
 
 * Fix `flake8` issues
```

### Comparing `vutils-testing-0.6.2/LICENSE` & `vutils-testing-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vutils-testing-0.6.2/PKG-INFO` & `vutils-testing-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: vutils-testing
-Version: 0.6.2
+Version: 1.0.0
 Summary: Auxiliary library for writing tests
 Home-page: https://github.com/i386x/vutils-testing
 Author: Jiří Kučera
 Author-email: sanczes@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/i386x/vutils-testing/issues
 Project-URL: Source, https://github.com/i386x/vutils-testing
 Keywords: testing,mocking,unit testing
 Platform: any
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `vutils-testing-0.6.2/README.md` & `vutils-testing-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `vutils-testing-0.6.2/pyproject.toml` & `vutils-testing-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vutils-testing-0.6.2/setup.cfg` & `vutils-testing-1.0.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 url = https://github.com/i386x/vutils-testing
 project_urls = 
 	Bug Reports = https://github.com/i386x/vutils-testing/issues
 	Source = https://github.com/i386x/vutils-testing
 author = Jiří Kučera
 author_email = sanczes@gmail.com
 classifiers = 
-	Development Status :: 1 - Planning
+	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	Intended Audience :: Information Technology
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
@@ -62,14 +62,18 @@
 metadata = True
 restructuredtext = False
 strict = True
 
 [sdist]
 formats = zip, gztar
 
+[coverage:report]
+exclude_lines = 
+	^if TYPE_CHECKING:$
+
 [flake8]
 filename = *.py,*.pyi,*.pyw
 select = E,F,W,C,G,Y
 enable-extensions = G,Y
 max-line-length = 79
 max-doc-length = 79
 extend-ignore = E203, E302, W503
```

### Comparing `vutils-testing-0.6.2/src/vutils/testing/__init__.pyi` & `vutils-testing-1.0.0/src/vutils/testing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `vutils-testing-0.6.2/src/vutils/testing/mock.py` & `vutils-testing-1.0.0/src/vutils/testing/mock.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,99 +24,117 @@
     )
 else:
     make_patch = unittest.mock.patch
 
 
 def make_mock(*args: object, **kwargs: object) -> "Mock":
     """
-    Make the `unittest.mock.Mock` object.
+    Make the :class:`unittest.mock.Mock` object.
 
-    :param args: Positional arguments to be passed to the `unittest.mock.Mock`
-        constructor
-    :param kwargs: Key-value arguments to be passed to the `unittest.mock.Mock`
-        constructor
-    :return: the `unittest.mock.Mock` object
+    :param args: Positional arguments to be passed to the
+        :class:`unittest.mock.Mock` constructor
+    :param kwargs: Key-value arguments to be passed to the
+        :class:`unittest.mock.Mock` constructor
+    :return: the :class:`unittest.mock.Mock` object
     """
     return unittest.mock.Mock(*args, **kwargs)
 
 
 def make_callable(returns: "ReturnsType" = None) -> "Mock":
     """
-    Make the `unittest.mock.Mock` object that serves as a callable.
+    Make the :class:`unittest.mock.Mock` object that serves as a callable.
 
-    :param returns: If callable, *returns* is treated as the *side_effect*
-        parameter to `unittest.mock.Mock`. Otherwise, it is treated as the
-        *return_value* parameter
-    :return: the `unittest.mock.Mock` object representing the callable
+    :param returns: If callable, :arg:`returns` is treated as the
+        :arg:`side_effect:unittest.mock.Mock` parameter to
+        :class:`unittest.mock.Mock`. Otherwise, it is treated as
+        the :arg:`return_value:unittest.mock.Mock` parameter
+    :return: the :class:`unittest.mock.Mock` object representing the callable
     """
     if callable(returns):
         return unittest.mock.Mock(side_effect=returns)
     return unittest.mock.Mock(return_value=returns)
 
 
 class PatchSpec:
-    """Holds the patch specification."""
+    """
+    Holds the patch specification.
+
+    :ivar __target: The target to be patched
+    :ivar __setupfunc: The setup function for the patch
+    :ivar __kwargs: Key-value arguments passed to :func:`unittest.mock.patch`
+    """
 
+    __target: object
+    __setupfunc: "SetupFuncType"
+    __kwargs: "KwArgsType"
     __slots__ = ("__target", "__setupfunc", "__kwargs")
 
     def __init__(
         self, target: object, setupfunc: "SetupFuncType", **kwargs: object
     ) -> None:
         """
         Initialize the patch specification.
 
         :param target: The target to be patched
         :param setupfunc: The function used to setup the patch
-        :param kwargs: Additional arguments passed to `unittest.mock.patch`
+        :param kwargs: Additional key-value arguments passed to
+            :func:`unittest.mock.patch`
         """
-        self.__target: object = target
-        self.__setupfunc: "SetupFuncType" = setupfunc
-        self.__kwargs: "KwArgsType" = kwargs
+        self.__target = target
+        self.__setupfunc = setupfunc
+        self.__kwargs = kwargs
 
     def __call__(self) -> "PatchType":
         """
         Create the patcher from the specification.
 
         :return: the patcher
 
         The patcher is created in four steps:
 
-        #. `unittest.mock.Mock` object is created
-        #. if *new* is in *kwargs*, the mock object becomes *new*
-        #. if *setupfunc* is not `None`, the mock object is passed to it; the
-           *setupfunc* can then adjust the object
-        #. the patcher is created by calling `unittest.mock.patch` with
-           *target*, the mock object, and additional arguments given by
-           *kwargs*, respectively
+        #. :class:`unittest.mock.Mock` object is created
+        #. if *new* is in :arg:`kwargs:.PatchSpec.__init__`, the mock object
+           becomes *new*
+        #. if :arg:`setupfunc:.PatchSpec.__init__` is not :obj:`None`, the mock
+           object is passed to it; the :arg:`setupfunc:.PatchSpec.__init__` can
+           then adjust the object
+        #. the patcher is created by calling :func:`unittest.mock.patch` with
+           :arg:`target:.PatchSpec.__init__`, the mock object, and additional
+           arguments given by :arg:`kwargs:.PatchSpec.__init__`, respectively
         """
         kwargs: "KwArgsType" = self.__kwargs.copy()
         mock: "MockableType" = kwargs.pop("new", make_mock())
         if self.__setupfunc is not None:
             self.__setupfunc(mock)
         return make_patch(self.__target, mock, **kwargs)
 
 
 class PatchingContextManager:
-    """Context manager that handles the patching."""
+    """
+    Context manager that handles the patching.
 
+    :ivar __patchers: The list of patchers
+    """
+
+    __patchers: "list[PatchType]"
     __slots__ = ("__patchers",)
 
     def __init__(self, patchers: Iterable["PatchType"]) -> None:
         """
         Initialize the context manager.
 
         :param patchers: The list of patchers
         """
-        self.__patchers: "list[PatchType]" = list(patchers)
+        self.__patchers = list(patchers)
 
     def __enter__(self) -> "PatchingContextManager":
         """
         Apply patches.
 
-        :return: *self*
+        :return: the instance that receives this method call (a.k.a *self*)
         """
         for patcher in self.__patchers:
             patcher.start()
         return self
 
     def __exit__(self, *args: object) -> None:
         """
@@ -128,19 +146,21 @@
             patcher.stop()
 
 
 class PatcherFactory:
     r"""
     Factory for creating patchers.
 
+    :ivar __specs: The list of patch specifications
+
     This factory allows to create and apply the set of patches simultaneously,
     omitting the nested ``with`` statements for every patch. In the following
     example, it is demonstrated how this class can be used to test the sending
     colored text to the standard output. First, define the factory that patch
-    the `colorama` and `sys` modules::
+    the :mod:`colorama` and :mod:`sys` modules::
 
         import colorama
         import io
         import sys
 
 
         class MyPatcher(PatcherFactory):
@@ -172,37 +192,40 @@
 
             with patcher.patch():
                 echo_red(message)
 
             assert patcher.stream.getvalue() == f"<c:red>{message}</c>\n"
 
     The patches are applied in order as their specifications were added by
-    `add_spec`.
+    :meth:`~.PatcherFactory.add_spec`.
     """
 
+    __specs: "list[PatchSpec]"
     __slots__ = ("__specs",)
 
     def __init__(self) -> None:
         """Initialize the factory."""
-        self.__specs: "list[PatchSpec]" = []
+        self.__specs = []
         self.setup()
 
     def add_spec(
         self,
         target: object,
         setupfunc: "SetupFuncType" = None,
         **kwargs: object,
     ) -> "PatcherFactory":
         """
         Add the patch specification to the factory.
 
         :param target: The target to be patched
-        :param setupfunc: The function used to setup the patch, see `PatchSpec`
-        :param kwargs: Additional arguments to `unittest.mock.patch`
-        :return: *self*
+        :param setupfunc: The function used to setup the patch, see
+            :class:`.PatchSpec`
+        :param kwargs: Additional key-value arguments to
+            :func:`unittest.mock.patch`
+        :return: the instance that receives this method call (a.k.a *self*)
         """
         self.__specs.append(PatchSpec(target, setupfunc, **kwargs))
         return self
 
     def setup(self) -> None:
         """Set up the factory."""
```

### Comparing `vutils-testing-0.6.2/src/vutils/testing/testcase.py` & `vutils-testing-1.0.0/src/vutils/testing/testcase.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,49 +2,49 @@
 # File:    ./src/vutils/testing/testcase.py
 # Author:  Jiří Kučera <sanczes AT gmail.com>
 # Date:    2021-09-02 00:59:53 +0200
 # Project: vutils-testing: Auxiliary library for writing tests
 #
 # SPDX-License-Identifier: MIT
 #
-"""Extended `unittest.TestCase`."""
+"""Extended :class:`unittest.TestCase`."""
 
 import unittest
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from unittest.mock import Mock
 
 
 class TestCase(unittest.TestCase):
-    """Extended `unittest.TestCase`."""
+    """Extended :class:`unittest.TestCase`."""
 
     __slots__ = ()
 
     @staticmethod
     def assert_called_with(
         mock: "Mock", *args: object, **kwargs: object
     ) -> None:
         """
         Check and reset the mock call.
 
         :param mock: The mock object
-        :param args: Expected arguments
+        :param args: Expected positional arguments
         :param kwargs: Expected key-value arguments
 
         Check whether the mock object has been called with given arguments and
         reset it.
         """
         mock.assert_called_once_with(*args, **kwargs)
         mock.reset_mock()
 
     @staticmethod
     def assert_not_called(mock: "Mock") -> None:
         """
-        Check that *mock* has not been called.
+        Check that :arg:`mock` has not been called.
 
         :param mock: The mock object
 
         Check whether the mock object has not been called and reset it.
         """
         mock.assert_not_called()
         mock.reset_mock()
```

### Comparing `vutils-testing-0.6.2/src/vutils/testing/utils.py` & `vutils-testing-1.0.0/src/vutils/testing/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import importlib
 from typing import TYPE_CHECKING, Iterable, cast
 
 from vutils.testing.mock import PatcherFactory
 
 if TYPE_CHECKING:
+    from types import ModuleType
     from unittest import TestCase
 
     from vutils.testing import (
         ArgsType,
         BasesType,
         ExcSpecType,
         FuncType,
@@ -35,15 +36,15 @@
 ) -> type:
     """
     Make a new type.
 
     :param name: The type name
     :param bases: The type's bases
     :param members: The definition of type's members and methods
-    :param kwargs: Additional arguments passed to `type`
+    :param kwargs: Additional key-value arguments passed to :class:`type`
     :return: the new type
 
     This function becomes handy when creating types used as test data. For
     instance, instead of ::
 
         class ErrorA(Exception):
             pass
@@ -74,106 +75,129 @@
         bases = (bases,)
     if members is None:
         members = {}
     return type(name, bases, members, **kwargs)
 
 
 class LazyInstanceMethod:
-    """Lazy instance method."""
+    """
+    Lazy instance method.
+
+    :ivar __owner: The lazy instance proxy
+    :ivar __name: The method name
+    """
 
+    __owner: "LazyInstanceProxy"
+    __name: str
     __slots__ = ("__owner", "__name")
 
     def __init__(self, owner: "LazyInstanceProxy", name: str) -> None:
         """
         Initialize the method wrapper.
 
         :param owner: The owner of the lazy instance method
         :param name: The name of the method
         """
-        self.__owner: "LazyInstanceProxy" = owner
-        self.__name: str = name
+        self.__owner = owner
+        self.__name = name
 
     def __call__(self, *args: object, **kwargs: object) -> object:
         """
         Delegate the call to the proper method of the instance.
 
-        :param args: Arguments passed to the method
+        :param args: Positional arguments passed to the method
         :param kwargs: Key-value arguments passed to the method
         :return: the value returned by the method
         """
         inst: object = self.__owner.get_instance()
         return cast("FuncType", getattr(inst, self.__name))(*args, **kwargs)
 
 
 class LazyInstanceProxy:
-    """Lazy instance proxy."""
+    """
+    Lazy instance proxy.
+
+    :ivar __owner: The lazy instance
+    :ivar __args: Positional arguments passed to the instance constructor
+    :ivar __kwargs: Key-value arguments passed to the instance constructor
+    """
 
+    __owner: "LazyInstance"
+    __args: "ArgsType"
+    __kwargs: "KwArgsType"
     __slots__ = ("__owner", "__args", "__kwargs")
 
     def __init__(
         self,
         owner: "LazyInstance",
         args: "ArgsType",
         kwargs: "KwArgsType",
     ) -> None:
         """
         Initialize the proxy.
 
         :param owner: The owner of the proxy
-        :param args: Arguments to be passed to the constructor during the
-            initialization of the instance
+        :param args: Positional arguments to be passed to the constructor
+            during the initialization of the instance
         :param kwargs: Key-value arguments to be passed to the constructor
             during the initialization of the instance
         """
-        self.__owner: "LazyInstance" = owner
-        self.__args: "ArgsType" = args
-        self.__kwargs: "KwArgsType" = kwargs
+        self.__owner = owner
+        self.__args = args
+        self.__kwargs = kwargs
 
     def get_instance(self) -> object:
         """
         Get the instance via proxy.
 
         :return: the initialized or cached instance
         """
         return self.__owner.get_instance(self, self.__args, self.__kwargs)
 
     def __getattr__(self, name: str) -> "LazyInstanceMethod | object":
         """
-        Get the value of the *name* member of the instance.
+        Get the value of the :arg:`name` member of the instance.
 
         :param name: The name of the member
         :return: the value of the member
 
-        If the value of *name* is callable, wrap it inside
-        `LazyInstanceMethod`.
+        If the value of :arg:`name` is callable, wrap it inside
+        :class:`.LazyInstanceMethod`.
         """
         if self.__owner.has_method(name):
             return LazyInstanceMethod(self, name)
         inst: object = self.get_instance()
         return cast(object, getattr(inst, name))
 
 
 class LazyInstance:
     r"""
     Support lazy initialization.
 
+    :ivar __cache: The lazy instance proxy to the instance mapping
+    :ivar __klass: The class of the instance
+    :ivar __initialize_once: When :obj:`False`, :meth:`.get_instance` creates
+        a new instance every time when called
+
     Object is constructed/initialized at time when its member function is
     called. Example::
 
         foo_factory = LazyInstance(Foo, initialize_once=False)
         foo = foo_factory.create(1, bar=2)
         test(foo.quux)
 
     when ``test`` calls ``foo.quux``, ``Foo(1, bar=2)`` is invoked first
     to make the instance of ``Foo`` and to cache the instance inside
     ``foo_factory``. Then, from this instance, ``quux`` is invoked. Since
-    ``foo_factory`` was created with *initialize_once* property set to `False`,
-    ``foo`` is initialized every time when ``foo.quux`` is invoked.
+    ``foo_factory`` was created with :attr:`.__initialize_once` property set
+    to :obj:`False`, ``foo`` is initialized every time when ``foo.quux`` is
+    invoked.
 
-    The story behind `LazyInstance`: consider the following snippet of code::
+    The story behind :class:`.LazyInstance`: consider the following snippet of
+    code::
 
         class Foo:
             def __init__(self):
                 self.stream = sys.stderr
 
             def greet(self):
                 self.stream.write("Hello!\n")
@@ -186,152 +210,165 @@
 
     in this scenario::
 
         mystream = io.StringIO()
         foo = Foo()
         test(foo.greet, mystream)
 
-    ``Hello!\n`` will be send to `sys.stderr` since the patching has been done
-    too late. This is where `LazyInstance` comes to help us::
+    ``Hello!\n`` will be send to :obj:`sys.stderr` since the patching has been
+    done too late. This is where :class:`.LazyInstance` comes to help us::
 
         mystream = io.StringIO()
         foo_factory = LazyInstance(Foo)
         foo = foo_factory.create()
         test(foo.greet, mystream)
 
-    now,  ``Hello!\n`` is written to ``mystream`` as expected.
+    now, ``Hello!\n`` is written to ``mystream`` as expected.
     """
 
+    __cache: "dict[LazyInstanceProxy, object]"
+    __klass: "TypeType"
+    __initialize_once: bool
     __slots__ = ("__cache", "__klass", "__initialize_once")
 
     def __init__(
         self, klass: "TypeType", initialize_once: bool = False
     ) -> None:
         """
         Initialize the lazy instance.
 
         :param klass: The class from which instance is created
         :param initialize_once: The flag saying that instance should be created
             and initialized only once
         """
-        self.__cache: "dict[LazyInstanceProxy, object]" = {}
-        self.__klass: "TypeType" = klass
-        self.__initialize_once: bool = initialize_once
+        self.__cache = {}
+        self.__klass = klass
+        self.__initialize_once = initialize_once
 
     def get_instance(
         self,
         proxy: "LazyInstanceProxy",
         args: "ArgsType",
         kwargs: "KwArgsType",
     ) -> object:
         """
         Get the instance.
 
         :param proxy: The lazy instance proxy
-        :param args: Arguments passed to the constructor during the
+        :param args: Positional arguments passed to the constructor during the
             initialization of the instance
         :param kwargs: Key-value arguments passed to the constructor during the
             initialization of the instance
         :return: the initialized or cached instance
 
         If the instance is not created or initialized or if it is to be needed
-        reinitialized, do it. *args* and *kwargs* are passed to the
+        reinitialized, do it. :arg:`args` and :arg:`kwargs` are passed to the
         constructor.
         """
         if proxy not in self.__cache or not self.__initialize_once:
             self.__cache[proxy] = self.__klass(*args, **kwargs)
         return self.__cache[proxy]
 
     def has_method(self, name: str) -> bool:
         """
-        Test whether the class has method *name*.
+        Test whether the class has method :arg:`name`.
 
         :param name: The name of the method
-        :return: `True` if the class has the method called *name*
+        :return: :obj:`True` if the class has the method called :arg:`name`
         """
         return callable(cast(object, getattr(self.__klass, name, None)))
 
     def create(self, *args: object, **kwargs: object) -> "LazyInstanceProxy":
         """
         Create the proxy of the lazy instance.
 
-        :param args: Arguments passed to the constructor during the
+        :param args: Positional arguments passed to the constructor during the
             initialization of the instance
         :param kwargs: Key-value arguments passed to the constructor during the
             initialization of the instance
         :return: the proxy of the lazy instance
         """
         return LazyInstanceProxy(self, args, kwargs)
 
 
 class AssertRaises:
     """
     Wrapper that asserts that callable raises.
 
+    :ivar __testcase: The test case
+    :ivar __func: The callable object to be tested
+    :ivar __raises: Expected exceptions
+    :ivar __exception: The caught exception
+
     Consider there are two functions ``func1`` and ``func2`` that are very
     similar to each other except ``func2`` raises an exception. Since their
     similarity, the test case defines a function ``run_and_verify(func)`` which
     runs them and test their results and side-effects. However, since ``func2``
     raises an exception, ``run_and_verify(func2)`` fails. To deal with such a
-    situation, `AssertRaises` can be used::
+    situation, :class:`.AssertRaises` can be used::
 
         class MyTestCase(CommonTestCase):
 
             def test_funcs(self):
                 wfunc2 = AssertRaises(self, func2, FooError)
 
                 # run_and_verify is defined in CommonTestCase
                 self.run_and_verify(func1)
                 # Does not fail, exception is caught and stored for later use
                 self.run_and_verify(wfunc2)
                 # Analyze caught exception
                 self.assertEqual(wfunc2.get_exception().detail, "foo")
     """
 
+    __testcase: "TestCase"
+    __func: "FuncType"
+    __raises: "ExcSpecType"
+    __exception: "Exception | None"
     __slots__ = ("__testcase", "__func", "__raises", "__exception")
 
     def __init__(
         self, testcase: "TestCase", func: "FuncType", raises: "ExcSpecType"
     ) -> None:
         """
         Initialize the wrapper.
 
         :param testcase: The test case
         :param func: The callable object to be tested
-        :param raises: The expected exceptions
+        :param raises: Expected exceptions
         """
-        self.__testcase: "TestCase" = testcase
-        self.__func: "FuncType" = func
+        self.__testcase = testcase
+        self.__func = func
         if not isinstance(raises, tuple):
             raises = (raises,)
-        self.__raises: "ExcSpecType" = raises
-        self.__exception: "Exception | None" = None
+        self.__raises = raises
+        self.__exception = None
 
     def get_exception(self) -> "Exception | None":
         """
         Get the caught exception.
 
         :return: the caught exception object
 
-        When called, *self* is cleared (the next call will return `None`).
+        When called, the caught exception storage is cleared (the next call
+        will return :obj:`None`).
         """
         exc: "Exception | None" = self.__exception
         self.__exception = None
         return exc
 
     def __call__(self, *args: object, **kwargs: object) -> None:
         """
         Invoke the callable object.
 
         :param args: Positional arguments
         :param kwargs: Key-value arguments
 
-        Invoke the callable object with *args* and *kwargs*, catch and store
-        the exception. Fail if the exception is not raised by the callable
-        object or if it is not in the list of expected exceptions.
+        Invoke the callable object with :arg:`args` and :arg:`kwargs`, catch
+        and store the exception. Fail if the exception is not raised by the
+        callable object or if it is not in the list of expected exceptions.
         """
         with self.__testcase.assertRaises(self.__raises) as catcher:
             self.__func(*args, **kwargs)
         self.__exception = catcher.exception
 
 
 class TypingPatcher(PatcherFactory):
@@ -341,18 +378,18 @@
 
     def setup(self) -> None:
         """Set up the patcher."""
         self.add_spec("typing.TYPE_CHECKING", new=True)
 
     def extend(self, target: str, symbols: Iterable[str]) -> None:
         """
-        Specify patches for *symbols*.
+        Specify patches for :arg:`target`.
 
         :param target: The target module
-        :param symbols: The list of symbols to be patched in the *target*
+        :param symbols: The list of symbols to be patched in the :arg:`target`
         """
         for symbol in symbols:
             self.add_spec(f"{target}.{symbol}", new=symbol, create=True)
 
 
 class ClassLikeSymbol(type):
     """Meta class for class-like symbols."""
@@ -380,27 +417,28 @@
         if typing.TYPE_CHECKING:
             from foo import _TypeA, _TypeB
 
     in ``foo.bar`` module covered by tests, call ::
 
         cover_typing("foo.bar", ["_TypeA", "_TypeB"])
 
-    Since this function uses `importlib.reload`, unpleasant side-effects may
-    occur. To avoid this, put your `cover_typing` code into separate file and
-    tell to ``pytest`` to run it as last (use ``pytest-order`` plugin) ::
+    Since this function uses :func:`importlib.reload`, unpleasant side-effects
+    may occur. To avoid this, put your :func:`.cover_typing` code into a
+    separate file and tell to ``pytest`` to run it as last (use
+    ``pytest-order`` plugin) ::
 
         import pytest
 
         from vutils.testing.utils import cover_typing
 
 
         @pytest.mark.order("last")
         def test_typing_code_is_covered():
             cover_typing("foo.bar", ["_TypeA", "_TypeB"])
     """
-    module = importlib.import_module(name)
-    patcher = TypingPatcher()
+    module: "ModuleType" = importlib.import_module(name)
+    patcher: "TypingPatcher" = TypingPatcher()
     patcher.extend(name.rsplit(".", 1)[0], symbols)
 
     with patcher.patch():
         importlib.reload(module)
     importlib.reload(module)
```

### Comparing `vutils-testing-0.6.2/src/vutils_testing.egg-info/PKG-INFO` & `vutils-testing-1.0.0/src/vutils_testing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: vutils-testing
-Version: 0.6.2
+Version: 1.0.0
 Summary: Auxiliary library for writing tests
 Home-page: https://github.com/i386x/vutils-testing
 Author: Jiří Kučera
 Author-email: sanczes@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/i386x/vutils-testing/issues
 Project-URL: Source, https://github.com/i386x/vutils-testing
 Keywords: testing,mocking,unit testing
 Platform: any
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `vutils-testing-0.6.2/src/vutils_testing.egg-info/SOURCES.txt` & `vutils-testing-1.0.0/src/vutils_testing.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -17,13 +17,12 @@
 src/vutils_testing.egg-info/PKG-INFO
 src/vutils_testing.egg-info/SOURCES.txt
 src/vutils_testing.egg-info/dependency_links.txt
 src/vutils_testing.egg-info/not-zip-safe
 src/vutils_testing.egg-info/requires.txt
 src/vutils_testing.egg-info/top_level.txt
 tests/unit/__init__.py
-tests/unit/common.py
-tests/unit/test_coverage.py
 tests/unit/test_mock.py
 tests/unit/test_testcase.py
 tests/unit/test_utils.py
-tests/unit/test_version.py
+tests/unit/test_version.py
+tests/unit/utils.py
```

### Comparing `vutils-testing-0.6.2/tests/unit/test_mock.py` & `vutils-testing-1.0.0/tests/unit/test_mock.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,28 @@
 # File:    ./tests/unit/test_mock.py
 # Author:  Jiří Kučera <sanczes AT gmail.com>
 # Date:    2021-09-16 22:48:07 +0200
 # Project: vutils-testing: Auxiliary library for writing tests
 #
 # SPDX-License-Identifier: MIT
 #
-"""Test `vutils.testing.mock` module."""
+"""
+Test :mod:`vutils.testing.mock` module.
+
+.. |make_mock| replace:: :func:`~vutils.testing.mock.make_mock`
+.. |make_callable| replace:: :func:`~vutils.testing.mock.make_callable`
+.. |PatchSpecTestCase| replace:: :class:`.PatchSpecTestCase`
+.. |PatcherFactoryTestCase| replace:: :class:`.PatcherFactoryTestCase`
+.. |PatchSpec| replace:: :class:`~vutils.testing.mock.PatchSpec`
+.. |setupfunc| replace::
+   :arg:`setupfunc:vutils.testing.mock.PatchSpec.__init__`
+.. |PatchingContextManager| replace::
+   :class:`~vutils.testing.mock.PatchingContextManager`
+.. |PatcherFactory| replace:: :class:`~vutils.testing.mock.PatcherFactory`
+"""
 
 import unittest.mock
 
 from vutils.testing.mock import (
     PatcherFactory,
     PatchingContextManager,
     PatchSpec,
@@ -18,83 +31,91 @@
     make_mock,
 )
 from vutils.testing.testcase import TestCase
 from vutils.testing.utils import make_type
 
 
 class MakeMockTestCase(TestCase):
-    """Test case for `make_mock`."""
+    """Test case for |make_mock|."""
 
     __slots__ = ()
 
     def test_make_mock(self):
         """
-        Test `make_mock`.
+        Test |make_mock|.
 
-        Test whether `make_mock` returns the instance of `unittest.mock.Mock`.
+        Test whether |make_mock| returns the instance of
+        :class:`unittest.mock.Mock`.
         """
         self.assertIsInstance(make_mock(), unittest.mock.Mock)
 
     def test_make_mock_with_args(self):
         """
-        Test `make_mock` with arguments.
+        Test |make_mock| with arguments.
 
-        Test whether arguments are passed to `unittest.mock.Mock`.
+        Test whether arguments are passed to :class:`unittest.mock.Mock`.
         """
         text = "abc"
         mock = make_mock(["write"])
 
         with self.assertRaises(AttributeError):
             mock.write_()
 
         mock.write(text)
         self.assert_called_with(mock.write, text)
 
 
 class MakeCallableTestCase(TestCase):
-    """Test case for `make_callable`."""
+    """Test case for |make_callable|."""
 
     __slots__ = ()
 
     def test_make_callable_with_no_args(self):
         """
-        Test `make_callable` with no arguments.
+        Test |make_callable| with no arguments.
 
-        With no arguments, `make_callable` will produce callable
-        `unittest.mock.Mock` object returning `None`.
+        With no arguments, |make_callable| will produce callable
+        :class:`unittest.mock.Mock` object returning :obj:`None`.
         """
         func = make_callable()
 
         self.assertIsNone(func())
 
     def test_make_callable_with_non_callable(self):
         """
-        Test `make_callable` with non-callable.
+        Test |make_callable| with non-callable.
 
-        This will produce `unittest.mock.Mock` object that returns the
+        This will produce :class:`unittest.mock.Mock` object that returns the
         non-callable object as its value.
         """
         func = make_callable(3)
 
         self.assertEqual(func(), 3)
 
     def test_make_callable_with_callable(self):
         """
-        Test `make_callable` with callable.
+        Test |make_callable| with callable.
 
-        This will produce `unittest.mock.Mock` object that uses callable to
-        perform the side-effect.
+        This will produce :class:`unittest.mock.Mock` object that uses callable
+        to perform the side-effect.
         """
         func = make_callable(lambda x: x + 1)
 
         self.assertEqual(func(3), 4)
 
 
 class PatchXTestCaseBase(TestCase):
-    """Base class for `PatchSpecTestCase` and `PatcherFactoryTestCase`."""
+    """
+    Base class for |PatchSpecTestCase| and |PatcherFactoryTestCase|.
+
+    :ivar mock: The :class:`unittest.mock.Mock` object used as an argument
+    :ivar patch: The mocked :func:`unittest.mock.patch`
+    :ivar patcher: The patcher
+    :ivar target: The target to be patched
+    """
 
     __slots__ = ("mock", "patch", "patcher", "target")
 
     def setUp(self):
         """Set up the test."""
         self.mock = make_mock()
         mock_mock = make_callable(lambda *x: self.mock)
@@ -104,48 +125,48 @@
             .add_spec("vutils.testing.mock.make_patch", new=self.patch)
             .add_spec("unittest.mock.Mock", new=mock_mock)
         )
         self.target = "__main__.print"
 
 
 class PatchSpecTestCase(PatchXTestCaseBase):
-    """Test case for `PatchSpec`."""
+    """Test case for |PatchSpec|."""
 
     __slots__ = ()
 
     def test_patch_spec_without_setupfunc(self):
-        """Test `PatchSpec` with *setupfunc* set to `None`."""
+        """Test |PatchSpec| with |setupfunc| set to :obj:`None`."""
         with self.patcher.patch():
             PatchSpec(self.target, None)()
 
         self.assert_called_with(self.patch, self.target, self.mock)
 
     def test_patch_spec_with_setupfunc(self):
-        """Test `PatchSpec` with *setupfunc* given."""
+        """Test |PatchSpec| with |setupfunc| given."""
         setupfunc = make_callable()
 
         with self.patcher.patch():
             PatchSpec(self.target, setupfunc)()
 
         self.assert_called_with(setupfunc, self.mock)
         self.assert_called_with(self.patch, self.target, self.mock)
 
     def test_patch_spec_with_all_args(self):
-        """Test `PatchSpec` with all arguments given."""
+        """Test |PatchSpec| with all arguments given."""
         setupfunc = make_callable()
         new = 1
 
         with self.patcher.patch():
             PatchSpec(self.target, setupfunc, new=new, create=True)()
 
         self.assert_called_with(setupfunc, new)
         self.assert_called_with(self.patch, self.target, new, create=True)
 
     def test_patch_spec_for_side_effects(self):
-        """Test `PatchSpec` for side effects."""
+        """Test |PatchSpec| for side effects."""
         new = 1
         patchspec = PatchSpec(self.target, None, new=new)
 
         with self.patcher.patch():
             patchspec()
 
         self.assert_called_with(self.patch, self.target, new)
@@ -153,20 +174,20 @@
         with self.patcher.patch():
             patchspec()
 
         self.assert_called_with(self.patch, self.target, new)
 
 
 class PatchingContextManagerTestCase(TestCase):
-    """Test case for `PatchingContextManager`."""
+    """Test case for |PatchingContextManager|."""
 
     __slots__ = ()
 
     def test_patching_context_manager(self):
-        """Test `PatchingContextManager`."""
+        """Test |PatchingContextManager|."""
         func = make_callable()
 
         mock_a = make_mock()
         mock_a.start = make_callable(lambda *x: func(1))
         mock_a.stop = make_callable(lambda *x: func(2))
 
         mock_b = make_mock()
@@ -184,20 +205,20 @@
                 unittest.mock.call(4),
                 unittest.mock.call(2),
             ],
         )
 
 
 class PatcherFactoryTestCase(PatchXTestCaseBase):
-    """Test case for `PatcherFactory`."""
+    """Test case for |PatcherFactory|."""
 
     __slots__ = ()
 
     def test_patcher_factory(self):
-        """Test `PatcherFactory`."""
+        """Test |PatcherFactory|."""
         setupfunc_a = make_callable()
         setupfunc_b = make_callable()
         patcher_klass = make_type(
             "FooPatcher", PatcherFactory, {"setup": setupfunc_a}
         )
 
         new = 42
```

### Comparing `vutils-testing-0.6.2/tests/unit/test_testcase.py` & `vutils-testing-1.0.0/tests/unit/test_testcase.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,27 +2,35 @@
 # File:    ./tests/unit/test_testcase.py
 # Author:  Jiří Kučera <sanczes AT gmail.com>
 # Date:    2021-09-11 08:30:17 +0200
 # Project: vutils-testing: Auxiliary library for writing tests
 #
 # SPDX-License-Identifier: MIT
 #
-"""Test `vutils.testing.testcase` module."""
+"""
+Test :mod:`vutils.testing.testcase` module.
+
+.. |TestCase| replace:: :class:`~vutils.testing.testcase.TestCase`
+.. |assert_called_with| replace::
+   :meth:`~vutils.testing.testcase.TestCase.assert_called_with`
+.. |assert_not_called| replace::
+   :meth:`~vutils.testing.testcase.TestCase.assert_not_called`
+"""
 
 from vutils.testing.mock import make_mock
 from vutils.testing.testcase import TestCase
 
 
 class TestCaseTestCase(TestCase):
-    """Test case for `TestCase`."""
+    """Test case for |TestCase|."""
 
     __slots__ = ()
 
     def test_assert_called_with(self):
-        """Test `TestCase.assert_called_with` method."""
+        """Test |assert_called_with| method."""
         mock = make_mock(["foo"])
 
         mock.foo()
         self.assert_called_with(mock.foo)
 
         mock.foo(1, 2)
         self.assert_called_with(mock.foo, 1, 2)
@@ -30,11 +38,11 @@
         mock.foo(bar=3, baz=4)
         self.assert_called_with(mock.foo, bar=3, baz=4)
 
         mock.foo(5, quux=6)
         self.assert_called_with(mock.foo, 5, quux=6)
 
     def test_assert_not_called(self):
-        """Test `TestCase.assert_not_called` method."""
+        """Test |assert_not_called| method."""
         mock = make_mock(["foo"])
 
         self.assert_not_called(mock.foo)
```

### Comparing `vutils-testing-0.6.2/tests/unit/test_version.py` & `vutils-testing-1.0.0/tests/unit/test_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # File:    ./tests/unit/test_version.py
 # Author:  Jiří Kučera <sanczes AT gmail.com>
 # Date:    2021-06-21 23:58:43 +0200
 # Project: vutils-testing: Auxiliary library for writing tests
 #
 # SPDX-License-Identifier: MIT
 #
-"""Test `vutils.testing.version` module."""
+"""Test :mod:`vutils.testing.version` module."""
 
 from vutils.testing.testcase import TestCase
 from vutils.testing.version import __version__
 
 
 class VersionTestCase(TestCase):
     """Test case for version."""
```

### Comparing `vutils-testing-0.6.2/tox.ini` & `vutils-testing-1.0.0/tox.ini`

 * *Files 0% similar despite different names*

```diff
@@ -5,26 +5,27 @@
 # Project: vutils-testing: Auxiliary library for writing tests
 # Brief:   Configuration for tox
 #
 # SPDX-License-Identifier: MIT
 #
 
 [tox]
+requires =
+    pip >= 19.2
+    setuptools >= 65.5.1
+    wheel >= 0.38.1
 envlist =
     py{37,38,39,310}, linters
 skip_missing_interpreters = True
 
 [testenv]
 passenv = *
 description =
     {envname}: Run unit tests for {envname}
 deps =
-    pip >= 19.2
-    setuptools >= 65.5.1
-    wheel >= 0.38.1
     safety
     pytest
     pytest-cov
     pytest-order
     coveralls
 commands =
     safety check --full-report
```

