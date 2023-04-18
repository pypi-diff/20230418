# Comparing `tmp/poocr-0.0.4.tar.gz` & `tmp/poocr-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poocr-0.0.4.tar", last modified: Sun Apr 16 10:13:24 2023, max compression
+gzip compressed data, was "poocr-0.0.5.tar", last modified: Tue Apr 18 14:43:22 2023, max compression
```

## Comparing `poocr-0.0.4.tar` & `poocr-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 10:13:24.294331 poocr-0.0.4/
--rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poocr-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     4588 2023-04-16 10:13:24.294331 poocr-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4067 2023-04-02 05:09:27.000000 poocr-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 10:13:24.231025 poocr-0.0.4/poocr/
--rw-rw-rw-   0        0        0      523 2023-03-25 11:20:01.000000 poocr-0.0.4/poocr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 10:13:24.274127 poocr-0.0.4/poocr/api/
--rw-rw-rw-   0        0        0      265 2023-03-25 11:08:27.000000 poocr-0.0.4/poocr/api/__init__.py
--rw-rw-rw-   0        0        0    20975 2023-01-30 12:39:04.000000 poocr-0.0.4/poocr/api/ocr.py
--rw-rw-rw-   0        0        0    10432 2023-04-16 10:12:06.000000 poocr-0.0.4/poocr/api/ocr2excel.py
-drwxrwxrwx   0        0        0        0 2023-04-16 10:13:24.278120 poocr-0.0.4/poocr/core/
--rw-rw-rw-   0        0        0     4071 2023-01-30 12:39:04.000000 poocr-0.0.4/poocr/core/OCR.py
--rw-rw-rw-   0        0        0      223 2023-01-22 06:56:13.000000 poocr-0.0.4/poocr/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 10:13:24.287268 poocr-0.0.4/poocr/lib/
--rw-rw-rw-   0        0        0     1017 2023-01-28 13:49:56.000000 poocr-0.0.4/poocr/lib/CommonUtils.py
--rw-rw-rw-   0        0        0     1132 2023-01-30 12:39:04.000000 poocr-0.0.4/poocr/lib/Config.py
--rw-rw-rw-   0        0        0      852 2023-01-30 12:39:04.000000 poocr-0.0.4/poocr/lib/Const.py
--rw-rw-rw-   0        0        0        0 2023-01-22 10:20:33.000000 poocr-0.0.4/poocr/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 10:13:24.268112 poocr-0.0.4/poocr.egg-info/
--rw-rw-rw-   0        0        0     4588 2023-04-16 10:13:24.000000 poocr-0.0.4/poocr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      455 2023-04-16 10:13:24.000000 poocr-0.0.4/poocr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 10:13:24.000000 poocr-0.0.4/poocr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-16 09:44:14.000000 poocr-0.0.4/poocr.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       40 2023-04-16 10:13:24.000000 poocr-0.0.4/poocr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-16 10:13:24.000000 poocr-0.0.4/poocr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      732 2023-04-16 10:13:24.298346 poocr-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poocr-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 10:13:24.292810 poocr-0.0.4/tests/
--rw-rw-rw-   0        0        0      181 2023-01-30 12:39:04.000000 poocr-0.0.4/tests/__init__.py
--rw-rw-rw-   0        0        0      823 2023-04-16 09:36:45.000000 poocr-0.0.4/tests/test_tencent.py
+drwxrwxrwx   0        0        0        0 2023-04-18 14:43:22.636200 poocr-0.0.5/
+-rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poocr-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     4588 2023-04-18 14:43:22.636200 poocr-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4067 2023-04-02 05:09:27.000000 poocr-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 14:43:22.589504 poocr-0.0.5/poocr/
+-rw-rw-rw-   0        0        0      523 2023-03-25 11:20:01.000000 poocr-0.0.5/poocr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 14:43:22.620671 poocr-0.0.5/poocr/api/
+-rw-rw-rw-   0        0        0      265 2023-03-25 11:08:27.000000 poocr-0.0.5/poocr/api/__init__.py
+-rw-rw-rw-   0        0        0    20975 2023-01-30 12:39:04.000000 poocr-0.0.5/poocr/api/ocr.py
+-rw-rw-rw-   0        0        0     3113 2023-04-18 14:41:56.000000 poocr-0.0.5/poocr/api/ocr2excel.py
+drwxrwxrwx   0        0        0        0 2023-04-18 14:43:22.623670 poocr-0.0.5/poocr/core/
+-rw-rw-rw-   0        0        0     4071 2023-01-30 12:39:04.000000 poocr-0.0.5/poocr/core/OCR.py
+-rw-rw-rw-   0        0        0      223 2023-01-22 06:56:13.000000 poocr-0.0.5/poocr/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 14:43:22.631179 poocr-0.0.5/poocr/lib/
+-rw-rw-rw-   0        0        0     1017 2023-01-28 13:49:56.000000 poocr-0.0.5/poocr/lib/CommonUtils.py
+-rw-rw-rw-   0        0        0     1132 2023-01-30 12:39:04.000000 poocr-0.0.5/poocr/lib/Config.py
+-rw-rw-rw-   0        0        0      852 2023-01-30 12:39:04.000000 poocr-0.0.5/poocr/lib/Const.py
+-rw-rw-rw-   0        0        0        0 2023-01-22 10:20:33.000000 poocr-0.0.5/poocr/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 14:43:22.615635 poocr-0.0.5/poocr.egg-info/
+-rw-rw-rw-   0        0        0     4588 2023-04-18 14:43:22.000000 poocr-0.0.5/poocr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      455 2023-04-18 14:43:22.000000 poocr-0.0.5/poocr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 14:43:22.000000 poocr-0.0.5/poocr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-18 14:43:22.000000 poocr-0.0.5/poocr.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       40 2023-04-18 14:43:22.000000 poocr-0.0.5/poocr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-18 14:43:22.000000 poocr-0.0.5/poocr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      732 2023-04-18 14:43:22.638198 poocr-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poocr-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 14:43:22.634219 poocr-0.0.5/tests/
+-rw-rw-rw-   0        0        0      181 2023-01-30 12:39:04.000000 poocr-0.0.5/tests/__init__.py
+-rw-rw-rw-   0        0        0      823 2023-04-16 09:36:45.000000 poocr-0.0.5/tests/test_tencent.py
```

### Comparing `poocr-0.0.4/LICENSE` & `poocr-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `poocr-0.0.4/PKG-INFO` & `poocr-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poocr
-Version: 0.0.4
+Version: 0.0.5
 Summary: pip install poocr
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poocr/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poocr/blob/main/README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poocr Version: 0.0.4 Summary: pip install poocr
+Metadata-Version: 2.1 Name: poocr Version: 0.0.5 Summary: pip install poocr
 Home-page: https://www.python-office.com/ Author: CoderWanFeng Author-email:
 1957875073@qq.com License: MIT Project-URL: Bug Tracker, https://github.com/
 CoderWanFeng/poocr/issues Project-URL: Documentation, https://github.com/
 CoderWanFeng/poocr/blob/main/README.md Project-URL: Source Code, https://
 github.com/CoderWanFeng/poocr Platform: any Requires-Python: >=3.7 Description-
 Content-Type: text/markdown License-File: LICENSE
 [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/ads%2F1040x100-
```

### Comparing `poocr-0.0.4/README.md` & `poocr-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `poocr-0.0.4/poocr/__init__.py` & `poocr-0.0.5/poocr/__init__.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.4/poocr/api/ocr.py` & `poocr-0.0.5/poocr/api/ocr.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.4/poocr/core/OCR.py` & `poocr-0.0.5/poocr/core/OCR.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.4/poocr/lib/CommonUtils.py` & `poocr-0.0.5/poocr/lib/CommonUtils.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.4/poocr/lib/Config.py` & `poocr-0.0.5/poocr/lib/Config.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.4/poocr/lib/Const.py` & `poocr-0.0.5/poocr/lib/Const.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.4/poocr.egg-info/PKG-INFO` & `poocr-0.0.5/poocr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poocr
-Version: 0.0.4
+Version: 0.0.5
 Summary: pip install poocr
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poocr/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poocr/blob/main/README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poocr Version: 0.0.4 Summary: pip install poocr
+Metadata-Version: 2.1 Name: poocr Version: 0.0.5 Summary: pip install poocr
 Home-page: https://www.python-office.com/ Author: CoderWanFeng Author-email:
 1957875073@qq.com License: MIT Project-URL: Bug Tracker, https://github.com/
 CoderWanFeng/poocr/issues Project-URL: Documentation, https://github.com/
 CoderWanFeng/poocr/blob/main/README.md Project-URL: Source Code, https://
 github.com/CoderWanFeng/poocr Platform: any Requires-Python: >=3.7 Description-
 Content-Type: text/markdown License-File: LICENSE
 [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/ads%2F1040x100-
```

### Comparing `poocr-0.0.4/setup.cfg` & `poocr-0.0.5/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f6f 6372 0d0a 7665 7273 696f   = poocr..versio
-00000020: 6e20 3d20 302e 302e 340d 0a64 6573 6372  n = 0.0.4..descr
+00000020: 6e20 3d20 302e 302e 350d 0a64 6573 6372  n = 0.0.5..descr
 00000030: 6970 7469 6f6e 203d 2070 6970 2069 6e73  iption = pip ins
 00000040: 7461 6c6c 2070 6f6f 6372 0d0a 6c6f 6e67  tall poocr..long
 00000050: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000060: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 00000090: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
```

### Comparing `poocr-0.0.4/tests/test_tencent.py` & `poocr-0.0.5/tests/test_tencent.py`

 * *Files identical despite different names*

