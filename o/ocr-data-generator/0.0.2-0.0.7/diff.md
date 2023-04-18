# Comparing `tmp/ocr_data_generator-0.0.2.tar.gz` & `tmp/ocr_data_generator-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocr_data_generator-0.0.2.tar", last modified: Tue Apr 18 18:53:14 2023, max compression
+gzip compressed data, was "ocr_data_generator-0.0.7.tar", last modified: Tue Apr 18 19:13:53 2023, max compression
```

## Comparing `ocr_data_generator-0.0.2.tar` & `ocr_data_generator-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 18:53:14.735845 ocr_data_generator-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-04-18 16:11:33.000000 ocr_data_generator-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      754 2023-04-18 18:53:14.735845 ocr_data_generator-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-04-18 16:17:49.000000 ocr_data_generator-0.0.2/README.md
--rw-rw-rw-   0        0        0       95 2023-04-18 16:11:33.000000 ocr_data_generator-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      647 2023-04-18 18:53:14.738845 ocr_data_generator-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      969 2023-04-18 16:18:25.000000 ocr_data_generator-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 18:53:14.654513 ocr_data_generator-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-18 18:53:14.724103 ocr_data_generator-0.0.2/src/ocr_data_generator/
--rw-rw-rw-   0        0        0      233 2023-04-18 16:28:30.000000 ocr_data_generator-0.0.2/src/ocr_data_generator/__init__.py
--rw-rw-rw-   0        0        0     2305 2023-04-18 16:13:56.000000 ocr_data_generator-0.0.2/src/ocr_data_generator/background_generator.py
--rw-rw-rw-   0        0        0     3848 2023-04-18 18:31:22.000000 ocr_data_generator-0.0.2/src/ocr_data_generator/drawer.py
--rw-rw-rw-   0        0        0     1278 2023-04-18 18:30:20.000000 ocr_data_generator-0.0.2/src/ocr_data_generator/font_generator.py
--rw-rw-rw-   0        0        0     2386 2023-04-18 18:30:54.000000 ocr_data_generator-0.0.2/src/ocr_data_generator/foreground_generator.py
--rw-rw-rw-   0        0        0     1510 2023-04-18 16:13:56.000000 ocr_data_generator-0.0.2/src/ocr_data_generator/painter.py
--rw-rw-rw-   0        0        0      918 2023-04-18 16:25:00.000000 ocr_data_generator-0.0.2/src/ocr_data_generator/sample_generator.py
--rw-rw-rw-   0        0        0      305 2023-04-18 16:32:53.000000 ocr_data_generator-0.0.2/src/ocr_data_generator/word_generator.py
-drwxrwxrwx   0        0        0        0 2023-04-18 18:53:14.734838 ocr_data_generator-0.0.2/src/ocr_data_generator.egg-info/
--rw-rw-rw-   0        0        0      754 2023-04-18 18:53:14.000000 ocr_data_generator-0.0.2/src/ocr_data_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      556 2023-04-18 18:53:14.000000 ocr_data_generator-0.0.2/src/ocr_data_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 18:53:14.000000 ocr_data_generator-0.0.2/src/ocr_data_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-18 18:53:14.000000 ocr_data_generator-0.0.2/src/ocr_data_generator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:13:53.894967 ocr_data_generator-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-18 19:13:41.000000 ocr_data_generator-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-18 19:13:53.894967 ocr_data_generator-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-18 19:13:41.000000 ocr_data_generator-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-18 19:13:41.000000 ocr_data_generator-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-18 19:13:53.894967 ocr_data_generator-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-18 19:13:41.000000 ocr_data_generator-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:13:53.894967 ocr_data_generator-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:13:53.894967 ocr_data_generator-0.0.7/src/ocr_data_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-18 19:13:41.000000 ocr_data_generator-0.0.7/src/ocr_data_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-18 19:13:41.000000 ocr_data_generator-0.0.7/src/ocr_data_generator/background_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-04-18 19:13:41.000000 ocr_data_generator-0.0.7/src/ocr_data_generator/drawer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-18 19:13:41.000000 ocr_data_generator-0.0.7/src/ocr_data_generator/font_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-04-18 19:13:41.000000 ocr_data_generator-0.0.7/src/ocr_data_generator/foreground_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-18 19:13:41.000000 ocr_data_generator-0.0.7/src/ocr_data_generator/painter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-18 19:13:41.000000 ocr_data_generator-0.0.7/src/ocr_data_generator/sample_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-18 19:13:41.000000 ocr_data_generator-0.0.7/src/ocr_data_generator/word_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:13:53.894967 ocr_data_generator-0.0.7/src/ocr_data_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-18 19:13:53.000000 ocr_data_generator-0.0.7/src/ocr_data_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-18 19:13:53.000000 ocr_data_generator-0.0.7/src/ocr_data_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 19:13:53.000000 ocr_data_generator-0.0.7/src/ocr_data_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-18 19:13:53.000000 ocr_data_generator-0.0.7/src/ocr_data_generator.egg-info/top_level.txt
```

### Comparing `ocr_data_generator-0.0.2/LICENSE` & `ocr_data_generator-0.0.7/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright (c) 2018 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `ocr_data_generator-0.0.2/PKG-INFO` & `ocr_data_generator-0.0.7/src/ocr_data_generator.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,23 @@
-Metadata-Version: 2.1
-Name: ocr_data_generator
-Version: 0.0.2
-Summary: A small example package
-Home-page: https://github.com/pypa/sampleproject
-Author: baiyigali
-Author-email: 1304646911@qq.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Example Package
-
-This is a simple example package. You can use
-[Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
-to write your content.
-
-Change Logs
-- v0.0.1
-
-
+Metadata-Version: 2.1
+Name: ocr-data-generator
+Version: 0.0.7
+Summary: A small example package
+Home-page: https://github.com/pypa/sampleproject
+Author: baiyigali
+Author-email: 1304646911@qq.com
+Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Example Package
+
+This is a simple example package. You can use
+[Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
+to write your content.
+
+Change Logs
+- v0.0.1
```

### Comparing `ocr_data_generator-0.0.2/src/ocr_data_generator/background_generator.py` & `ocr_data_generator-0.0.7/src/ocr_data_generator/background_generator.py`

 * *Files identical despite different names*

### Comparing `ocr_data_generator-0.0.2/src/ocr_data_generator/drawer.py` & `ocr_data_generator-0.0.7/src/ocr_data_generator/drawer.py`

 * *Files identical despite different names*

### Comparing `ocr_data_generator-0.0.2/src/ocr_data_generator/font_generator.py` & `ocr_data_generator-0.0.7/src/ocr_data_generator/font_generator.py`

 * *Files identical despite different names*

### Comparing `ocr_data_generator-0.0.2/src/ocr_data_generator/foreground_generator.py` & `ocr_data_generator-0.0.7/src/ocr_data_generator/foreground_generator.py`

 * *Files identical despite different names*

### Comparing `ocr_data_generator-0.0.2/src/ocr_data_generator/painter.py` & `ocr_data_generator-0.0.7/src/ocr_data_generator/painter.py`

 * *Files identical despite different names*

### Comparing `ocr_data_generator-0.0.2/src/ocr_data_generator/sample_generator.py` & `ocr_data_generator-0.0.7/src/ocr_data_generator/sample_generator.py`

 * *Files identical despite different names*

### Comparing `ocr_data_generator-0.0.2/src/ocr_data_generator.egg-info/SOURCES.txt` & `ocr_data_generator-0.0.7/src/ocr_data_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

