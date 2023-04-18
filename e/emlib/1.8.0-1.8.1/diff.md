# Comparing `tmp/emlib-1.8.0.tar.gz` & `tmp/emlib-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emlib-1.8.0.tar", last modified: Wed Mar 29 14:13:14 2023, max compression
+gzip compressed data, was "emlib-1.8.1.tar", last modified: Tue Apr 18 11:11:24 2023, max compression
```

## Comparing `emlib-1.8.0.tar` & `emlib-1.8.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-03-29 14:13:14.481131 emlib-1.8.0/
--rw-rw-r--   0 em        (1000) em        (1000)     1065 2023-03-29 14:13:14.481131 emlib-1.8.0/PKG-INFO
--rwxrwxr-x   0 em        (1000) em        (1000)      612 2021-11-22 12:50:35.000000 emlib-1.8.0/README.rst
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-03-29 14:13:14.480131 emlib-1.8.0/emlib/
--rwxrwxr-x   0 em        (1000) em        (1000)      552 2021-11-22 12:50:35.000000 emlib-1.8.0/emlib/__init__.py
--rw-rw-r--   0 em        (1000) em        (1000)     9290 2022-02-28 20:16:06.000000 emlib-1.8.0/emlib/_dialogsqt.py
--rwxrwxr-x   0 em        (1000) em        (1000)     5276 2021-11-22 12:50:35.000000 emlib-1.8.0/emlib/calculus.py
--rwxrwxr-x   0 em        (1000) em        (1000)    13951 2021-11-22 12:51:36.000000 emlib-1.8.0/emlib/combinatorics.py
--rwxrwxr-x   0 em        (1000) em        (1000)    11691 2023-01-05 02:24:33.000000 emlib-1.8.0/emlib/containers.py
--rwxrwxr-x   0 em        (1000) em        (1000)     7381 2021-11-22 12:52:47.000000 emlib-1.8.0/emlib/csvtools.py
--rw-rw-r--   0 em        (1000) em        (1000)    14750 2023-03-29 14:12:27.000000 emlib-1.8.0/emlib/dialogs.py
--rw-rw-r--   0 em        (1000) em        (1000)    40862 2022-05-02 12:30:18.000000 emlib-1.8.0/emlib/doctools.py
--rwxrwxr-x   0 em        (1000) em        (1000)    11931 2023-02-13 09:29:14.000000 emlib-1.8.0/emlib/electronics.py
--rwxrwxr-x   0 em        (1000) em        (1000)     4783 2022-05-26 12:13:22.000000 emlib-1.8.0/emlib/filetools.py
--rw-rw-r--   0 em        (1000) em        (1000)     1666 2021-11-22 12:50:35.000000 emlib-1.8.0/emlib/graphlib.py
--rw-rw-r--   0 em        (1000) em        (1000)     4888 2021-11-22 12:50:35.000000 emlib-1.8.0/emlib/img.py
--rwxrwxr-x   0 em        (1000) em        (1000)    17569 2023-02-09 09:01:05.000000 emlib-1.8.0/emlib/iterlib.py
--rw-rw-r--   0 em        (1000) em        (1000)     3726 2021-11-22 12:50:35.000000 emlib-1.8.0/emlib/jsontools.py
--rwxrwxr-x   0 em        (1000) em        (1000)     1836 2022-12-11 17:42:25.000000 emlib-1.8.0/emlib/logutils.py
--rw-rw-r--   0 em        (1000) em        (1000)    20805 2023-02-27 19:03:05.000000 emlib-1.8.0/emlib/mathlib.py
--rw-rw-r--   0 em        (1000) em        (1000)    12649 2021-11-22 12:50:35.000000 emlib-1.8.0/emlib/matplotting.py
--rw-rw-r--   0 em        (1000) em        (1000)     3000 2021-11-22 12:50:35.000000 emlib-1.8.0/emlib/minizinctools.py
--rwxrwxr-x   0 em        (1000) em        (1000)    55359 2023-02-04 17:28:07.000000 emlib-1.8.0/emlib/misc.py
--rwxrwxr-x   0 em        (1000) em        (1000)     1361 2021-11-22 12:50:35.000000 emlib-1.8.0/emlib/net.py
--rw-rw-r--   0 em        (1000) em        (1000)     1824 2021-11-22 12:50:35.000000 emlib-1.8.0/emlib/numberseries.py
--rwxrwxr-x   0 em        (1000) em        (1000)     8133 2022-04-05 12:38:34.000000 emlib-1.8.0/emlib/numpytools.py
--rwxrwxr-x   0 em        (1000) em        (1000)     4890 2021-11-22 12:50:35.000000 emlib-1.8.0/emlib/numtheory.py
--rwxrwxr-x   0 em        (1000) em        (1000)     2126 2022-05-02 20:42:02.000000 emlib-1.8.0/emlib/parabolicinterpol.py
--rwxrwxr-x   0 em        (1000) em        (1000)     1840 2021-11-22 12:50:35.000000 emlib-1.8.0/emlib/readbytes.py
--rw-rw-r--   0 em        (1000) em        (1000)     2128 2021-11-22 12:50:35.000000 emlib-1.8.0/emlib/shelling.py
--rwxrwxr-x   0 em        (1000) em        (1000)     7950 2022-05-02 20:07:38.000000 emlib-1.8.0/emlib/smooth.py
--rwxrwxr-x   0 em        (1000) em        (1000)     7777 2022-05-02 20:07:38.000000 emlib-1.8.0/emlib/stochastic.py
--rw-rw-r--   0 em        (1000) em        (1000)     6060 2023-03-15 10:12:58.000000 emlib-1.8.0/emlib/textlib.py
--rwxrwxr-x   0 em        (1000) em        (1000)     1301 2022-05-02 19:50:30.000000 emlib-1.8.0/emlib/video.py
--rwxrwxr-x   0 em        (1000) em        (1000)     8527 2022-05-02 20:00:33.000000 emlib-1.8.0/emlib/xmlprinter.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-03-29 14:13:14.481131 emlib-1.8.0/emlib.egg-info/
--rw-rw-r--   0 em        (1000) em        (1000)     1065 2023-03-29 14:13:14.000000 emlib-1.8.0/emlib.egg-info/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)      779 2023-03-29 14:13:14.000000 emlib-1.8.0/emlib.egg-info/SOURCES.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2023-03-29 14:13:14.000000 emlib-1.8.0/emlib.egg-info/dependency_links.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2022-02-27 18:43:41.000000 emlib-1.8.0/emlib.egg-info/not-zip-safe
--rw-rw-r--   0 em        (1000) em        (1000)      117 2023-03-29 14:13:14.000000 emlib-1.8.0/emlib.egg-info/requires.txt
--rw-rw-r--   0 em        (1000) em        (1000)        6 2023-03-29 14:13:14.000000 emlib-1.8.0/emlib.egg-info/top_level.txt
--rwxrwxr-x   0 em        (1000) em        (1000)       61 2023-03-29 14:13:14.482131 emlib-1.8.0/setup.cfg
--rw-rw-r--   0 em        (1000) em        (1000)     1074 2023-03-29 14:13:03.000000 emlib-1.8.0/setup.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-18 11:11:24.140437 emlib-1.8.1/
+-rw-rw-r--   0 em        (1000) em        (1000)     1065 2023-04-18 11:11:24.141437 emlib-1.8.1/PKG-INFO
+-rwxrwxr-x   0 em        (1000) em        (1000)      612 2021-11-22 12:50:35.000000 emlib-1.8.1/README.rst
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-18 11:11:24.136437 emlib-1.8.1/emlib/
+-rwxrwxr-x   0 em        (1000) em        (1000)      552 2021-11-22 12:50:35.000000 emlib-1.8.1/emlib/__init__.py
+-rw-rw-r--   0 em        (1000) em        (1000)     9290 2022-02-28 20:16:06.000000 emlib-1.8.1/emlib/_dialogsqt.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     5276 2021-11-22 12:50:35.000000 emlib-1.8.1/emlib/calculus.py
+-rwxrwxr-x   0 em        (1000) em        (1000)    13951 2021-11-22 12:51:36.000000 emlib-1.8.1/emlib/combinatorics.py
+-rwxrwxr-x   0 em        (1000) em        (1000)    11691 2023-01-05 02:24:33.000000 emlib-1.8.1/emlib/containers.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     7381 2021-11-22 12:52:47.000000 emlib-1.8.1/emlib/csvtools.py
+-rw-rw-r--   0 em        (1000) em        (1000)    14750 2023-03-29 14:12:27.000000 emlib-1.8.1/emlib/dialogs.py
+-rw-rw-r--   0 em        (1000) em        (1000)    40862 2022-05-02 12:30:18.000000 emlib-1.8.1/emlib/doctools.py
+-rwxrwxr-x   0 em        (1000) em        (1000)    11931 2023-02-13 09:29:14.000000 emlib-1.8.1/emlib/electronics.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     4783 2022-05-26 12:13:22.000000 emlib-1.8.1/emlib/filetools.py
+-rw-rw-r--   0 em        (1000) em        (1000)     1666 2021-11-22 12:50:35.000000 emlib-1.8.1/emlib/graphlib.py
+-rw-rw-r--   0 em        (1000) em        (1000)     4888 2021-11-22 12:50:35.000000 emlib-1.8.1/emlib/img.py
+-rwxrwxr-x   0 em        (1000) em        (1000)    17569 2023-02-09 09:01:05.000000 emlib-1.8.1/emlib/iterlib.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3726 2021-11-22 12:50:35.000000 emlib-1.8.1/emlib/jsontools.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     1836 2022-12-11 17:42:25.000000 emlib-1.8.1/emlib/logutils.py
+-rw-rw-r--   0 em        (1000) em        (1000)    20805 2023-02-27 19:03:05.000000 emlib-1.8.1/emlib/mathlib.py
+-rw-rw-r--   0 em        (1000) em        (1000)    12649 2021-11-22 12:50:35.000000 emlib-1.8.1/emlib/matplotting.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3000 2021-11-22 12:50:35.000000 emlib-1.8.1/emlib/minizinctools.py
+-rwxrwxr-x   0 em        (1000) em        (1000)    57495 2023-04-18 11:09:30.000000 emlib-1.8.1/emlib/misc.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     1361 2021-11-22 12:50:35.000000 emlib-1.8.1/emlib/net.py
+-rw-rw-r--   0 em        (1000) em        (1000)     1824 2021-11-22 12:50:35.000000 emlib-1.8.1/emlib/numberseries.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     8133 2022-04-05 12:38:34.000000 emlib-1.8.1/emlib/numpytools.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     4890 2021-11-22 12:50:35.000000 emlib-1.8.1/emlib/numtheory.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     2126 2022-05-02 20:42:02.000000 emlib-1.8.1/emlib/parabolicinterpol.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     1840 2021-11-22 12:50:35.000000 emlib-1.8.1/emlib/readbytes.py
+-rw-rw-r--   0 em        (1000) em        (1000)     2128 2021-11-22 12:50:35.000000 emlib-1.8.1/emlib/shelling.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     7950 2022-05-02 20:07:38.000000 emlib-1.8.1/emlib/smooth.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     7777 2022-05-02 20:07:38.000000 emlib-1.8.1/emlib/stochastic.py
+-rw-rw-r--   0 em        (1000) em        (1000)     6060 2023-03-15 10:12:58.000000 emlib-1.8.1/emlib/textlib.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     1301 2022-05-02 19:50:30.000000 emlib-1.8.1/emlib/video.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     8527 2022-05-02 20:00:33.000000 emlib-1.8.1/emlib/xmlprinter.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-18 11:11:24.140437 emlib-1.8.1/emlib.egg-info/
+-rw-rw-r--   0 em        (1000) em        (1000)     1065 2023-04-18 11:11:23.000000 emlib-1.8.1/emlib.egg-info/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)      779 2023-04-18 11:11:24.000000 emlib-1.8.1/emlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2023-04-18 11:11:23.000000 emlib-1.8.1/emlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2022-02-27 18:43:41.000000 emlib-1.8.1/emlib.egg-info/not-zip-safe
+-rw-rw-r--   0 em        (1000) em        (1000)      117 2023-04-18 11:11:23.000000 emlib-1.8.1/emlib.egg-info/requires.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        6 2023-04-18 11:11:23.000000 emlib-1.8.1/emlib.egg-info/top_level.txt
+-rwxrwxr-x   0 em        (1000) em        (1000)       61 2023-04-18 11:11:24.141437 emlib-1.8.1/setup.cfg
+-rw-rw-r--   0 em        (1000) em        (1000)     1074 2023-04-18 11:10:58.000000 emlib-1.8.1/setup.py
```

### Comparing `emlib-1.8.0/PKG-INFO` & `emlib-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emlib
-Version: 1.8.0
+Version: 1.8.1
 Summary: Miscellaneous utilities
 Home-page: https://github.com/gesellkammer/emlib
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `emlib-1.8.0/README.rst` & `emlib-1.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/__init__.py` & `emlib-1.8.1/emlib/__init__.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/_dialogsqt.py` & `emlib-1.8.1/emlib/_dialogsqt.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/calculus.py` & `emlib-1.8.1/emlib/calculus.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/combinatorics.py` & `emlib-1.8.1/emlib/combinatorics.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/containers.py` & `emlib-1.8.1/emlib/containers.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/csvtools.py` & `emlib-1.8.1/emlib/csvtools.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/dialogs.py` & `emlib-1.8.1/emlib/dialogs.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/doctools.py` & `emlib-1.8.1/emlib/doctools.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/electronics.py` & `emlib-1.8.1/emlib/electronics.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/filetools.py` & `emlib-1.8.1/emlib/filetools.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/graphlib.py` & `emlib-1.8.1/emlib/graphlib.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/img.py` & `emlib-1.8.1/emlib/img.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/iterlib.py` & `emlib-1.8.1/emlib/iterlib.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/jsontools.py` & `emlib-1.8.1/emlib/jsontools.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/logutils.py` & `emlib-1.8.1/emlib/logutils.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/mathlib.py` & `emlib-1.8.1/emlib/mathlib.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/matplotting.py` & `emlib-1.8.1/emlib/matplotting.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/minizinctools.py` & `emlib-1.8.1/emlib/minizinctools.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/misc.py` & `emlib-1.8.1/emlib/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 import numpy as np
 from fractions import Fraction
 import numbers
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING or 'sphinx' in _sys.modules:
-    from typing import TypeVar, Sequence, Union
+    from typing import TypeVar, Sequence, Union, Optional, Callable, Any, Iterable
     T = TypeVar("T")
     T2 = TypeVar("T2")
     number_t = Union[float, numbers.Rational]
     
 
 # ------------------------------------------------------------
 #     CHUNKS
@@ -251,15 +251,15 @@
         return [convert(c) for c in _re.split('([0-9]+)', key)]
 
     if key is not None:
         return sorted(seq, key=lambda x: alphanum_key(key(x)))
     return sorted(seq, key=alphanum_key)
 
 
-def sort_natural_dict(d: Dict[str, Any], recursive=True) -> dict:
+def sort_natural_dict(d: dict[str, Any], recursive=True) -> dict:
     """
     sort dict d naturally and recursively
     """
     rows: list[tuple[str, Any]] = []
     if recursive:
         for key, value in d.items():
             if isinstance(value, dict):
@@ -268,15 +268,15 @@
         sorted_rows = sort_natural(rows, key=lambda row: row[0])
     else:
         keys = list(d.keys())
         sorted_rows = [(key, d[key]) for key in sort_natural(keys)]
     return dict(sorted_rows)
 
 
-def issorted(seq:list, key=None) -> bool:
+def issorted(seq: list, key=None) -> bool:
     """
     Returns True if seq is sorted
 
     Args:
         seq: the seq. to query
         key: an optional key to use
 
@@ -784,15 +784,15 @@
     True
     """
     out = dict1.copy()
     out.update(dict2)
     return out
 
 
-def moses(pred: Callable[[T], bool], seq: Iterator[T]
+def moses(pred: Callable[[T], bool], seq: Iterable[T]
           ) -> tuple[list[T], list[T]]:
     """
     Divides *seq* into two lists: filter(pred, seq), filter(not pred, seq)
 
     Args:
         pred: a function predicate
         seq: the seq. to divide
@@ -813,15 +813,15 @@
         if pred(x):
             trueitems.append(x)
         else:
             falseitems.append(x)
     return trueitems, falseitems
 
 
-def allequal(xs: Iterator) -> bool:
+def allequal(xs: Sequence) -> bool:
     """
     Return True if all elements in xs are equal
 
     Args:
         xs: the seq. to query
 
     Returns:
@@ -861,15 +861,14 @@
 
     .. note::
 
         the result will have the same type as *x*, so if *x* is float,
         the result will be float, if it is a Fraction, then the
         result will be a fraction
     """
-    assert isinstance(x, (float, number.Rational))
     t = x.__class__
     if nearest:
         return t(round((x - offset) / tick)) * tick + offset
     else:
         return t(int((x - offset) / tick)) * tick + offset
 
 
@@ -1696,16 +1695,78 @@
         # we are inside ipython so we can just call 'get_ipython'
         ip = get_ipython()   # type: ignore
         return ip.active_eventloop == "qt"
     else:
         return False
 
 
-def html_table(rows: list, headers: list[str], maxwidths:Optional[list[int]]=None,
-               rowstyles:Optional[list[str]]=None) -> str:
+def get_platform() -> tuple[str, str]:
+    """
+    Return a tuple (osname, architecture)
+
+    This attempts to improve upon `sysconfig.get_platform` by fixing some
+    issues when running a Python interpreter with a different architecture than
+    that of the system (e.g. 32bit on 64bit system, or a multiarch build),
+    which should return the machine architecture of the currently running
+    interpreter rather than that of the system (which didn't seem to work
+    properly). The reported machine architectures follow platform-specific
+    naming conventions (e.g. "x86_64" on Linux, but "x64" on Windows).
+
+    Returns:
+        a tuple (osname: str, architecture: str)
+
+
+    Example output strings for common platforms::
+
+        ("darwin", one of ppc|ppc64|i368|x86_64|arm64)
+        ("linux", one of i686|x86_64|armv7l|aarch64)
+        ("windows", one of x86|x64|arm32|arm64
+
+
+
+    """
+    import platform
+    import sysconfig
+
+    system = platform.system().lower()
+    machine = sysconfig.get_platform().split("-")[-1].lower()
+    is_64bit = _sys.maxsize > 2 ** 32
+
+    if system == "darwin": # get machine architecture of multiarch binaries
+        if any([x in machine for x in ("fat", "intel", "universal")]):
+            machine = platform.machine().lower()
+
+    elif system == "linux":  # fix running 32bit interpreter on 64bit system
+        if not is_64bit and machine == "x86_64":
+            machine = "i686"
+        elif not is_64bit and machine == "aarch64":
+            machine = "armv7l"
+
+    elif system == "windows": # return more precise machine architecture names
+        if machine == "amd64":
+            machine = "x64"
+        elif machine == "win32":
+            if is_64bit:
+                machine = platform.machine().lower()
+            else:
+                machine = "x86"
+
+    # some more fixes based on examples in https://en.wikipedia.org/wiki/Uname
+    if not is_64bit and machine in ("x86_64", "amd64"):
+        if any([x in system for x in ("cygwin", "mingw", "msys")]):
+            machine = "i686"
+        else:
+            machine = "i386"
+
+    return system, machine
+
+def html_table(rows: list, 
+               headers: list[str], 
+               maxwidths: Optional[list[int]]=None,
+               rowstyles: Optional[list[str]]=None) -> str:
     """
     Create a html table
 
     Args:
         rows: the rows of the table, where each row is a sequence of cells
         headers: a list of column names
         maxwidths: if given, a list of max widths for each column
```

### Comparing `emlib-1.8.0/emlib/net.py` & `emlib-1.8.1/emlib/net.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/numberseries.py` & `emlib-1.8.1/emlib/numberseries.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/numpytools.py` & `emlib-1.8.1/emlib/numpytools.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/numtheory.py` & `emlib-1.8.1/emlib/numtheory.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/parabolicinterpol.py` & `emlib-1.8.1/emlib/parabolicinterpol.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/readbytes.py` & `emlib-1.8.1/emlib/readbytes.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/shelling.py` & `emlib-1.8.1/emlib/shelling.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/smooth.py` & `emlib-1.8.1/emlib/smooth.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/stochastic.py` & `emlib-1.8.1/emlib/stochastic.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/textlib.py` & `emlib-1.8.1/emlib/textlib.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/video.py` & `emlib-1.8.1/emlib/video.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib/xmlprinter.py` & `emlib-1.8.1/emlib/xmlprinter.py`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/emlib.egg-info/PKG-INFO` & `emlib-1.8.1/emlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emlib
-Version: 1.8.0
+Version: 1.8.1
 Summary: Miscellaneous utilities
 Home-page: https://github.com/gesellkammer/emlib
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `emlib-1.8.0/emlib.egg-info/SOURCES.txt` & `emlib-1.8.1/emlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emlib-1.8.0/setup.py` & `emlib-1.8.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import os
 import sys
 
 from setuptools import setup
 
 readme = open('README.rst').read()
-version = (1, 8, 0)
+version = (1, 8, 1)
 
 setup(
     name='emlib',
     python_requires=">=3.9",
     version=".".join(map(str, version)),
     description='Miscellaneous utilities',
     long_description=readme,
```

